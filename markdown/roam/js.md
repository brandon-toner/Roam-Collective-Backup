- Please don't make changes here, instead suggest them using [this] process.
- Roam42
    - {{{[[roam/js]]}}}
        - ```javascript

var s = document.createElement('script');
	s.type = "text/javascript";
    s.src =  "https://roam42.glitch.me/main.js"
  // 	s.src =  "https://roam42-test.glitch.me/main.js"
  	s.async = true;
document.body.appendChild(s);
```
- RoamJS
    - {{[[roam/js]]}}
        - ```javascript
var installScript = name => {
  var existing = document.getElementById(name);
  if (existing) {
    return;
  }  
  var extension = document.createElement("script");      
  extension.type = "text/javascript";
  extension.src = `https://roamjs.com/${name}.js`;
  extension.async = true;
  extension.id = name;
  document.getElementsByTagName("head")[0].appendChild(extension);
};
installScript("mindmap");
installScript("query-builder");
installScript("query-tools");
installScript("slack");
installScript("sort-references");
installScript("tag-cycle");
installScript("wiki-data");
```
- Disable Intercom
    - {{{[[roam/js]]}}}
        - ```javascript
try{
  document.querySelector('.intercom-lightweight-app').remove();
} catch(e) {};```
