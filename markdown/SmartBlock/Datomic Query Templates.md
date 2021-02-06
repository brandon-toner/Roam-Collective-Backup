- Type:: #Meta
    - The code on this page was written by ZSolt and is further detailed [here](https://www.zsolt.blog/2021/01/Roam-Data-Structure-Query.html) — the below allows users to run and output datalog queries within the graph.
- # Common functions
    - {{[[roam/js]]}}
        - ```javascript
window.datomicQuery = {
  MAXROWS: 40,
  reg_fields_string: null,
  reg_fields: null,
  reg_field: null,
  reg_is_pull: null,
  field_names: [],
  output: '',
  
  init() {
    this.reg_fields_string = new RegExp(/\:find\s+(.+)/);
    this.reg_fields        = new RegExp(/(\?[^\s]+|\(pull.+\))/g);
    this.reg_field         = new RegExp(/\?([\w\d]+)\:?([\w\d]+)?/);
    this.reg_is_pull       = new RegExp(/(\(.+\))/);//(\(\s?pull.+\))
  },
  
  //Helper functions to get clickeable links
  getLocation(uid) {
    if (window.location.href.includes('/page/')) 
      return window.location.href.substring(window.location.origin.length+1,window.location.href.length-9)+uid;
    else
      return window.location.href.substring(window.location.origin.length+1,window.location.href.length)+'/page/'+uid
  },
  pageLink(title, uid) {
    return `[:a {:class "rm-page__title", :href "${this.getLocation(uid)}"} "${title}"]`;
  },
  toTwoDigits(number) {
    return  ("0" + number).slice(-2);
  },
  msToDate(ms) {
    dt = new Date(ms);
    month = this.toTwoDigits(dt.getMonth()+1);
    day = this.toTwoDigits(dt.getDate());
    year = dt.getFullYear();
    uid = [month,day,year].join('-');
    title = [year, month, day].join('-');
    return this.pageLink(title,uid);
  },

  //In the end only the "quotation mark" needs an escape character due to hiccup
  encodeString(s){ 
    return s.replace(/["]/g, function(i) {
      return '\\"';
    });
  },

  //Helper function to check if variable is a dictionary object
  isDict(v) {
    return typeof v==='object' && v!==null && !(v instanceof Array) && !(v instanceof Date);
  },

  //recursive function to process the result set tree
  printResult(o,new_lines) {
    //Dictionary
    if (this.isDict(o)) {
      s = '[:table {:class "detail"} [:tbody ';
      for (var key in o) {
        val = o[key];
        if (key == 'title') 
          if (o['uid'] !== undefined)
            val = this.pageLink(val,o['uid']);
        if (key == 'time') 
          val = this.msToDate(o[key]);
        s += `[:tr [:td {:class "key"} "${key}"][:td {:class "val"} ${(o[key] != val) ? val : this.printResult(val,new_lines)}]]`;
      }
      return s+']]';
    }
    //Array
    else if (o instanceof Array) {  
  	  s = (new_lines) ? '[:table [:tbody ' : '';
      for (let i=0;i<this.MAXROWS/4 && i<o.length;i++) {
      //for (e of o) {       
      	s += ((new_lines) ? '[:tr {:class "' +(i%2 ? 'even val"}':'odd val"}') : '[:td {:class "val"}') + this.printResult(o[i],!new_lines)+']';
      }
      return s + ((new_lines) ? ']]' : '');
    }
    //Value
    else
      if (o != null) 
      	return '"' + this.encodeString(o.toString()) + '"';
      else 
        return '""';
  },
    
  getParentBlock() {
    let uid = document.querySelector("textarea.rm-block-input").id;
    uid = uid.substring( uid.length -9);
    return s = window.roamAlphaAPI.q(`[:find ?s
  								:in $ ?uid
  								:where 
  								[?b :block/uid ?uid]
  								[?p :block/children ?b]
								[?p :block/string ?s]]`,uid);
  }, 

  buildTableHeader(query) {
    this.output = ':hiccup [:div "Click here to edit block..." [:br][:div {:class "scroller dont-focus-block"}  [:table [:tbody [:tr ';
    this.field_names = [];    
    let fields = Array.from(query.match(this.reg_fields_string)[1].matchAll(this.reg_fields));
	for (var f of fields) 
      if (f[0].match(this.reg_is_pull) != null) 
        this.field_names.push([f[0],'pull']);
      else {
        m = f[0].match(this.reg_field);
      this.field_names.push([m[1],(m[2] === undefined) ? '':m[2]]);
    }
    this.field_names.forEach(function(field,i) { 
      if (field[1]!='uid') 
        window.datomicQuery.output += '[:td {:class "head"} "'+field[0]+'"]';
    });
    this.output += ']';
  },

  processResults(results,query) {
    query = query.replaceAll('\n',' ').replace(':in','\n:in').replace(':where','\n:where');
    this.buildTableHeader(query);
    //The first two levels are handled differently to enable processing of page links at the top level
    for (let i=0;i<this.MAXROWS && i<results.length;i++) {
      let title = '';
      this.output += '[:tr {:class "' +(i%2 ? 'even"}':'odd"}');
      this.field_names.forEach(function(fn,j) {
        switch(fn[1]) {
          case 'name': title = results[i][j]; break;
          case 'uid' : window.datomicQuery.output +=  '[:td {:class "val"}' + window.datomicQuery.pageLink(title, results[i][j]) +']'; break;
          case 'date': window.datomicQuery.output +=  '[:td {:class "val"}' + window.datomicQuery.msToDate(results[i][j]) +']';   + ']'; break;  
          default:     window.datomicQuery.output +=  '[:td {:class "val"}' + window.datomicQuery.printResult(results[i][j],false) +']'; 
        }
      });
      this.output += ']';
    }
    return this.output;
  }
}

window.datomicQuery.init();
let css = window.document.styleSheets[0];
css.insertRule('table.detail { width:100%; border-style: solid; border-width: thin; }', css.cssRules.length);
css.insertRule('td.key { padding-right: 10px; filter: brightness(110%); vertical-align: top; }', css.cssRules.length);
css.insertRule('td.head { padding-right: 10px; background-color: rgba(0,0,0,0.15); filter: brightness(120%); font-weight: 800; vertical-align: top; }', css.cssRules.length);
css.insertRule('td.val { padding-right: 10px; vertical-align: top; }', css.cssRules.length);
css.insertRule('tr.odd { background: rgba(255,255,255,0.05); vertical-align: top; }', css.cssRules.length);
css.insertRule('tr.even { background-color: rgba(0,0,0,0.05); vertical-align: top;}', css.cssRules.length);
css.insertRule('div.scroller { width: 100%; max-height: 500px; overflow-y: hidden; overflow: auto; }', css.cssRules.length);```
- # Query execution
    - #42SmartBlock Datomic simple-query <%NOCURSOR%><%HIDE%>
        - 
            - <%J:```javascript
let reg_parent_string = new RegExp('\`\`\`clojure\\s(.+)\`\`\`','s');

let query;
try{
  query = window.datomicQuery.getParentBlock()[0][0].match(reg_parent_string)[1];
} catch (err) {
  return 'ERROR - make sure you run the query from a block nested immediately under your query. Also check that common functions on [[Template/Datomic Query]] are running.';
}

//Execute query
let results;
try { 	
  results = window.roamAlphaAPI.q(query);
} catch (err) {
  return err;
}

return window.datomicQuery.processResults(results,query) + ']]]]';```%>
    - #42SmartBlock Datomic advanced-query <%NOCURSOR%><%HIDE%>
        - 
            - <%J:```javascript
let reg_parent_string = new RegExp('\`\`\`javascript\\s(.+)\`\`\`','s');
let script_to_run;
try {
  script_to_run = window.datomicQuery.getParentBlock()[0][0].match(reg_parent_string)[1];
} catch (err) {
  return 'ERROR - make sure you run the query from a block nested immediately under your query. Also check that common functions on [[Template/Datomic Query]] are running.';
}

//Execute query
let res;
try {
  res = new Function(script_to_run.toString())();
} catch (err) {
  return err;
}
let query = res[0];
let results = res[1];

return window.datomicQuery.processResults(results,query) + ']]]]';```%>
- # Templates
    - #42SmartBlock Datomic simple-template <%NOCURSOR%>
        - ```javascript
let s = "\`\`\`clojure\n";
s += '[:find ?title:name ?title:uid ?time:date\n';
s += ' :where [?page :node/title ?title:name]\n';
s += '        [?page :block/uid ?title:uid]\n';
s += '        [?page :edit/time ?time:date]\n';
s += '        [(clojure.string/starts-with? ?title:name "roam/")]]';
s += "\`\`\`";
return s;```%>
            - {{CLICK TO RUN SIMPLE-QUERY:42SmartBlock:Datomic simple-query:42RemoveButton=false}}
    - #42SmartBlock Datomic advanced-template <%NOCURSOR%>
        - ```javascript
let s = "\`\`\`javascript\n";
s += "window.datomicQuery.MAXROWS = 40;\n\n";
s += "let rule = \`\`;\n\n";
s += "let query = `[:find ?title:name ?title:uid ?time:date\n";
s += "				:in $ ?namespace\n";
s += "				:where [?page :node/title ?title:name]\n";
s += "					   [?page :block/uid ?title:uid]\n";
s += "					   [?page :edit/time ?time:date]\n";
s += "					   [(clojure.string/starts-with? ?title:name ?namespace)]]`;\n\n";
s += "let results = window.roamAlphaAPI.q(query,'roam/');\n\n";
s += "return [query, results];";
s += "\`\`\`";
return s;```%>
            - {{CLICK TO RUN ADVANCED-QUERY:42SmartBlock:Datomic advanced-query:42RemoveButton=false}}
    - #42SmartBlock Remove query-template header <%NOCURSOR%> <%HIDE%>
        - <%J:```javascript
let txt = document.querySelector("textarea.rm-block-input").value;
txt = txt.substr(txt.indexOf('`'));
document.querySelector("textarea.rm-block-input").value = '';
return txt;```%>
    - Note:
        - ^^1.^^ If within the **[:find** clause you designate a field with **:name** (e.g. ?title:name) it must be followed by a field designated by **:uid** (e.g. ?title:uid), these two fields will be combined into a page link. 
        - ^^2.^^ Fields containing time data, designated with **:date** will be converted into a friendly format date including a link to the daily page.
        - ^^3.^^ Fields within a **(pull ) or an aggregate function e.g. (min )** will not be checked for :name :uid :date
