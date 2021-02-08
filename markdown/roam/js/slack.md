- Code:
    - {{[[roam/js]]}}
        - ```javascript
var existing = document.getElementById("slack");
if (!existing) {
  var extension = document.createElement("script");
  extension.src = "https://roamjs.com/slack.js";
  extension.id = "slack";
  extension.async = true;
  extension.type = "text/javascript";
  document.getElementsByTagName("head")[0].appendChild(extension);
}
```
- 
