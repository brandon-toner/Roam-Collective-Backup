- [42SmartBlock](<42SmartBlock.md>) 2nd Degree (Experimental)
    - <%SET:second_degree_page_name,<%INPUT:Enter Page Name for 2nd degree references%>%><%NOBLOCKOUTPUT%>
    - <%SET:second_degree_days_since,<%INPUT:Number of days since today%>%><%NOBLOCKOUTPUT%>
    - <%NOBLOCKOUTPUT%><%J:```javascript
var page_name = roam42.smartBlocks.activeWorkflow.vars["second_degree_page_name"];
let number_of_days_since = roam42.smartBlocks.activeWorkflow.vars["second_degree_days_since"];;

let from_time = new Date().setDate(new Date().getDate() - number_of_days_since);
let query = window.roamAlphaAPI.q(`[:find (pull ?e [{:block/parents [:node/title]}]) 
                                    :where[?e :block/refs ?ref][?ref :node/title "${page_name}"]]`);

let page_list = [];

query.forEach(result => {
    if (result[0].parents) {
       let page_title = result[0].parents[0].title; 
       page_list.push(page_title);  
    }
})

let results = window.roamAlphaAPI.q(`[:find (pull ?e [:block/uid]) :in $ [?page-list ...]
                                      :where [?e :block/refs ?refs][?refs :node/title ?page-list]
                                      [?refs :edit/time ?block_edit][(>= ?block_edit ${from_time})]]`, 
                                      page_list)
let uids = [];
results.forEach(result => uids.push(`((${result[0].uid}))`));

roam42.smartBlocks.activeWorkflow.vars["second_degree_uids"] =  uids;
roam42.smartBlocks.activeWorkflow.vars["second_degree_results_count"] =  uids.length;
roam42.smartBlocks.activeWorkflow.vars["second_degree_uids_counter"] = 0;

return ''```%>
    - <%REPEAT:<%GET:second_degree_results_count%>%><%J:```javascript
let vars = roam42.smartBlocks.activeWorkflow.vars;
let counter = vars['second_degree_uids_counter'];
roam42.smartBlocks.activeWorkflow.vars["second_degree_uids_counter"] = roam42.smartBlocks.activeWorkflow.vars["second_degree_uids_counter"] + 1;

if (vars['second_degree_uids'][counter] == null) {
  return '';
}
return vars['second_degree_uids'][counter];```%>

# Backlinks
## [January 30th, 2021](<January 30th, 2021.md>)
- [2nd-Degree Filter](<2nd-Degree Filter.md>)

