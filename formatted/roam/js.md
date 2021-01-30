- Please don't make changes here, instead suggest them using [this] process.
- [Roam42](<../Roam42.md>) Stable Build [Status](<../Status.md>)/Enabled
    - {{{[roam/js](<../roam/js.md>)}}}
        - ```javascript

// DISABLE FEATURES
// Remove two forward slashes from in front of name 
// of feature to DISABLE it
// Everything is enabled by default
window.disabledFeatures = [
  // 'quickReference',
   'turnDown',
  // 'dateProcessing',
  // 'lookupUI',
  // 'livePreview',
   'dailyNote',
   'templatePoc',
  // 'jumpToDate',
  // 'jumpNav',
];

// Live Preview - to change the defaults 
// 1) remove // in front of parameter to ACTIVATE the change
// 2) modify the value to change it's behavior
// width  = width of preview window
// height = height of preview window
// delay  = milliseconds of delay for preview to 
// 			fire (defaults to 200) can be set to 0
window.roam42LivePreview = {
  //width:	'400px',
  //height: '600px',
  delay: 500,
}


// Change the Deep navigation options
// activate-on-no-focus - activate navigation mode when body is focused (default: false)
// REMOVE // in front of setting to change it from default setting
window.roamNavigatorSettings = {
//   'activate-on-no-focus': true, 
}

var s = document.createElement('script')
	s.type = "text/javascript"
    s.src =  "https://roam42.glitch.me/main.js"
  //  s.src =  "https://roam42-test.glitch.me/main.js"
	s.async = true
document.getElementsByTagName('head')[0].appendChild(s)
```
- RoamJS Tag-Cycles [roam/js/tag-cycle](<../roam/js/tag-cycle.md>)
    - {{[roam/js](<../roam/js.md>)}}
        - ```javascript
var existing = document.getElementById("tag-cycle");
if (!existing) {
  var extension = document.createElement("script");
  extension.src = "https://roamjs.com/tag-cycle.js";
  extension.id = "tag-cycle";
  extension.async = false;
  extension.type = "text/javascript";
  document.getElementsByTagName("head")[0].appendChild(extension);
}```
- 

# Backlinks
## [January 25th, 2021](<January 25th, 2021.md>)
8. Added [roam/js](<../roam/js.md>)

## [roam/css](<roam/css.md>)
- **[Related](<../Related.md>):** [roam/js](<../roam/js.md>)

## [roam/js](<roam/js.md>)
- {{{[roam/js](<../roam/js.md>)}

- {{[roam/js](<../roam/js.md>)}
