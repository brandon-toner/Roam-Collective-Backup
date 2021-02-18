- Tags:: #Graph/Templates #SmartBlocks
- Created by:: [[Dharam]]
- Description::
    - Uses the [datalog query](((SIZjCeOS3))) built by [[David Vargas]] and turns the results into page titles.
- #[[Next Steps]]
    - {{[[TODO]]}} Add a total count of the results
    - {{[[DONE]]}} Add a header
    - {{[[TODO]]}} Do the same thing, but as a stable query rather than a populated report. #Q is this possible? I guess thats what [this](((SIZjCeOS3))) is.
- #42SmartBlock 2nd Deg Page Titles (Experimental) #Bookmarks
    - **Pages authored by graph members:**
        - <%NOBLOCKOUTPUT%><%J:```javascript
let results = window.roamAlphaAPI.q(`[:find ?n :where [?note :node/title ?n]
[?bb :block/page ?note] [?bb :block/refs ?p]
[?bb :block/refs ?c] [?c :node/title "Author"]
[?b :block/page ?p] [?b :block/refs ?t] [?b :block/refs ?tag]
[?t :node/title "Members"] [?tag :node/title "Tags"]]`);

let page_titles = [];
results.forEach(result => page_titles.push(`[[${result[0]}]]`));

roam42.smartBlocks.activeWorkflow.vars["second_degree_pages"] =  page_titles;
roam42.smartBlocks.activeWorkflow.vars["second_degree_results_count"] =  page_titles.length;
roam42.smartBlocks.activeWorkflow.vars["second_degree_pages_counter"] = 0;```%>
        - <%REPEAT:<%GET:second_degree_results_count%>%><%J:```javascript
let vars = roam42.smartBlocks.activeWorkflow.vars;
let counter = vars['second_degree_pages_counter'];
let page_name = vars['second_degree_pages'][counter];

roam42.smartBlocks.activeWorkflow.vars["second_degree_pages_counter"] = vars["second_degree_pages_counter"] + 1;

return page_name;```%>
