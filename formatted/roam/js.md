- Please don't make changes here, instead suggest them. [blk-gray](<../blk-gray.md>)
- Roam42
    - {{{[roam/js](<../roam/js.md>)}}}
        - ```javascript
var s = document.createElement('script');
	s.type = "text/javascript";
    s.src =  "https://roam42-test.glitch.me/main.js"
  // 	s.src =  "https://roam42-test.glitch.me/main.js"
  	s.async = true;
document.body.appendChild(s);
```
- RoamJS
    - {{[roam/js](<../roam/js.md>)}}
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
    - {{{[roam/js](<../roam/js.md>)}}}
        - ```javascript
try{
  document.querySelector('.intercom-lightweight-app').remove();
} catch(e) {};```

# Backlinks
## [Charles Farr](<Charles Farr.md>)
- {{[roam/js](<../roam/js.md>)}

## [February 23rd, 2021](<February 23rd, 2021.md>)
- ""{{{[roam/js](<../roam/js.md>)}

- ""{{[roam/js](<../roam/js.md>)}

- "{{{[roam/js](<../roam/js.md>)}

- "{{[roam/js](<../roam/js.md>)}

## [January 25th, 2021](<January 25th, 2021.md>)
8. Added [roam/js](<../roam/js.md>)

## [January 31st, 2021](<January 31st, 2021.md>)
- I think every person needs to activate the [roam/js](<../roam/js.md>)

## [Matthew Vogel](<Matthew Vogel.md>)
- {{[roam/js](<../roam/js.md>)}

- {{[roam/js](<../roam/js.md>)}

- {{[roam/js](<../roam/js.md>)}

- {{[roam/js](<../roam/js.md>)}

- {{[roam/js](<../roam/js.md>)}

- {{[roam/js](<../roam/js.md>)}

## [RC/Onboarding Seedpack](<RC/Onboarding Seedpack.md>)
- [roam/js](<../roam/js.md>)

- {{{[roam/js](<../roam/js.md>)}

## [SmartBlock/Datomic Query Templates](<SmartBlock/Datomic Query Templates.md>)
- {{[roam/js](<../roam/js.md>)}

## [Welcome](<Welcome.md>)
- "{{{[roam/js](<../roam/js.md>)}

## [roam/js](<roam/js.md>)
- {{{[roam/js](<../roam/js.md>)}

- {{[roam/js](<../roam/js.md>)}

- {{{[roam/js](<../roam/js.md>)}

