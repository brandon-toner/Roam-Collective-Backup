- Please don't make changes here, instead suggest them. #blk-gray
- Roam42
    - {{{[[roam/js]]}}}
        - ```javascript
var existing = document.getElementById("roamjs-roam42-main");
if (!existing) {
  var extension = document.createElement("script");
  extension.src = "https://roamjs.com/roam42/main.js";
  extension.id = "roamjs-roam42-main";
  extension.async = true;
  extension.type = "text/javascript";
  document.getElementsByTagName("head")[0].appendChild(extension);
}```
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
//installScript("mindmap");
installScript("query-builder");
//installScript("query-tools");
//installScript("slack");
installScript("sort-references");
installScript("tag-cycle");
//installScript("wiki-data");
```
- Disable Intercom
    - {{{[[roam/js]]}}}
        - ```javascript
try{
  document.querySelector('.intercom-lightweight-app').remove();
} catch(e) {};```
