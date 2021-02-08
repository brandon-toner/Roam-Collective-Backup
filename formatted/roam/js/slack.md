- Code:
    - {{[roam/js](<../../roam/js.md>)}}
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

# Backlinks
## [February 8th, 2021](<February 8th, 2021.md>)
- Added [roam/js/slack](<../../roam/js/slack.md>)

