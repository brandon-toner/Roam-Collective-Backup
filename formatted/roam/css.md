- [Announcements](<../Announcements.md>)
    - ## Please document any changes to the CSS under a `#[Change Log](<../Change Log.md>)` tag within your [DNP Section](<../DNP Section.md>)
- **[Related](<../Related.md>):** [roam/js](<../roam/js.md>)
- **[Table of Contents](<../Table of Contents.md>):**
    - [Tag Styling](((yAzEsiUsx))) ((This needs to be tidied up significantly... ((r1E6gBj56))))
        - [Collections Tags](((JNVnlLDxv))) 
        - [Notifications & Mentions](((01X6uO5N8)))
    - Other Styling
        - [External Links](((r3wJzzQJP)))
        - [Block Reference Styling](((xcLgPdvs0)))
        - [Nested Links](((y9rumn-yn)))
- **[Contents](<../Contents.md>):**
    - add `?disablejs=true&disablecss=true` to the end of your roam graph URL, to load without CSS or JS
    - **[Tips](<../Tips.md>):** Filter by [Status](<../Status.md>)/Enabled in roam/css to view active code. ((This is reliant on updating the tags as things are switched on/off; so may be unreliable))
    - Roam Full Site Themes [Status](<../Status.md>)/Disabled
        - Main CSS (modified [Leyendecker](<../Leyendecker.md>))
            - Core
                - ```ruby
*h1  {
  	font-size: 2.5em;
}

[roam-right-sidebar-content](<../roam-right-sidebar-content.md>) h1.rm-title-display {
  	font-size: 1.8em
}

h2,
h3,
h4,
h5,
h6 {
    font-family: "Lato", sans-serif;
    font-size: 3em;
}

.rm-page-ref-namespace-color {
  color: [2179F3](<../2179F3.md>) !important
}

.rm-query {
    border: 0.5px solid [e4e9ec](<../e4e9ec.md>);
    border-radius: 5px;
    
}

.rm-query .rm-query-title {
    background-color: [f7f8f8](<../f7f8f8.md>);
    padding: 0.8em;
    color: [d1dbe2](<../d1dbe2.md>);
    font-size: 80%;
}

.rm-reference-main.rm-query-content {
    padding: 0.8em;
}

.rm-reference-main .rm-reference-item .rm-block-text {
    font-size: 90%;
}

.rm-ref-page-view-title span {
    
}

.rm-reference-main .rm-reference-item .controls {
    margin-left: -1em;
}

.rm-ref-page-view {
    padding: 0.4em 0.2em;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
    padding: 6px;
}

div.flex-v-box.starred-pages-wrapper > div.flex-h-box > span {
    font-size: 14px !important;
    opacity: 80%;
    letter-spacing: 0.04em;
}

div.roam-sidebar-container.noselect > div > div {
    font-size: 14px !important;
    letter-spacing: 0.03em;
    
}

[block-input](<../block-input.md>) {
    background: white;
}

.roam-body [block-input](<../block-input.md>) > span > div {
    padding: 6px 24px;
    background: white;
}

span.bp3-icon-small.bp3-icon-star {
    display: none;
    visibility: hidden;
}

.roam-block {
    max-width: 850px;
}

[right-sidebar](<../right-sidebar.md>) > div {
    background-color: [f7f8fa](<../f7f8fa.md>);
    border-left: 1px solid [e9ebef](<../e9ebef.md>);
}
.controls .simple-bullet-outer .simple-bullet-inner {
    background-color: [e5e9f2](<../e5e9f2.md>);
}
.block-border-left {
    border-left: 1px solid [f3f6f7](<../f3f6f7.md>);
}
.kanban-board {
    background-color: [fff](<../fff.md>);
}
.kanban-card {
    background-color: white;
    margin: 8px;
    box-shadow: 0px 1px 2px [9eb3c0a8](<../9eb3c0a8.md>);
    padding: 10px;
    border-radius: 2px;
    line-height: 1.3em;
}
.kanban-title {
    text-align: center;
    font-weight: 600;
    font-size: 1.1em;
    opacity: 80%;
    color: [485f6f](<../485f6f.md>);
    padding-top: 8px;
    border-bottom: 1px solid [c5d1d8](<../c5d1d8.md>);
}
.kanban-column {
    background-color: [e7eff3](<../e7eff3.md>);
    margin: 0px 4px 0px 4px;
    padding: 4px;
    min-width: 200px;
    border-radius: 3px;
}
/*
.rm-block-ref::before {
    content: '';
    display: inline-block;
    width: 2px;
    border-radius: 40px;
    height: 12px;
    background: [ff913c](<../ff913c.md>);
    margin-right: 8px;
}*/

.rm-block-ref {
    border-bottom: none;
    font-size: 1em;
    color: [515e70](<../515e70.md>);
}

.rm-block-ref:hover {
    background: none;
    cursor: pointer;
}
.checkmark {
    background: [fff](<../fff.md>);
}
.check-container input:checked ~ .checkmark {
    background: [2179F3](<../2179F3.md>);
}
.check-container input:checked ~ .checkmark:after {
    border-color: [fff](<../fff.md>);
}
.rm-reference-item {
    margin-top: 8px;
    border-radius: 6px;
    border: 1px solid [e4e9ee](<../e4e9ee.md>);
    margin-right: 8px;
    flex: 1 1 100%;
    word-break: break-word;
    background-color: [f7f9fb](<../f7f9fb.md>);
    padding: 8px;
}

.rm-level2 {
    font-size: 1.5em;
}
.rm-level3 {
    color: [939aae](<../939aae.md>);
    font-weight: 400;
    font-size: 1.3em;
}
.rm-page-ref {
    color: [4C616A](<../4C616A.md>);
}
.rm-page-ref-link-color {
    color: [2179F3](<../2179F3.md>);
    font-weight: 600;
}
a {
    color: [2179F3](<../2179F3.md>);
}
.intercom-app,
.intercom-launcher-frame,
[intercom-container](<../intercom-container.md>) {
    display: none !important;
}

/* Left Sidebar reformatting */

.roam-body .roam-app .roam-sidebar-container {
    background-color: white;
    border-right: 1px [eee](<../eee.md>) solid;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page,
.roam-body .roam-app .roam-sidebar-container > * {
    opacity: 80%;
    box-shadow: none;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
    background: white;
    color: black;
    opacity: 100%;
}
[buffer](<../buffer.md>).tall {
    height: calc(100vh - 50px) !important;
}
.check-container {
    padding-right: 4px;
}
span.rm-page-ref {
    border-radius: 2px;
    padding-left: 1px;
    padding-right: 1px;
}
.content span.rm-page-ref {
    padding: 4px 1px 1px;
    /* required for fixing azo */
}
.center-proj {
    text-align: center;
}```
            - Pomodoro 
                - ```css
.rm-pomodoro {
    background: [fff](<../fff.md>) !important;
    color: [ff4747](<../ff4747.md>) !important;
    padding: 4px 14px;
    line-height: 2em;
    font-weight: 600;
    border-radius: 2em;
    border: 1px solid [ff474770](<../ff474770.md>);
}

.rm-pomodoro {
    background: [ff6956](<../ff6956.md>) !important;
    color: [fff](<../fff.md>) !important;
    padding: 4px 14px;
    line-height: 2em;
    font-weight: 600;
    border-radius: 2em;
    border: 1px solid [ed5845](<../ed5845.md>);
}

.rm-pomodoro::first-letter {
  margin-right: 8px;
}```
    - ## Settings
        - Colors
            - Color Scheme
                - > Use names for consistent colors throughout your them
                - Base
                    - ```css
:root {
  --cl-white:			[ffffff](<../ffffff.md>);
  --cl-gray-50:			[f4f5f5](<../f4f5f5.md>);
  --cl-gray-100:		[e5e6e6](<../e5e6e6.md>);
  --cl-gray-200: 		[dcdcdc](<../dcdcdc.md>);
  --cl-gray-300: 		[bdbdbd](<../bdbdbd.md>);
  --cl-gray-400: 		[99999d](<../99999d.md>);
  --cl-gray-500: 		[797a79](<../797a79.md>);
  --cl-gray-600: 		[646464](<../646464.md>);
  --cl-gray-700: 		[454545](<../454545.md>);
  --cl-gray-800: 		[272727](<../272727.md>);
  --cl-gray-900:		[1a1a1a](<../1a1a1a.md>);
  --cl-black:			[000000](<../000000.md>);
  --cl-green-700: 		[1a8917](<../1a8917.md>);
  --cl-blue-50:			[e8f2ff](<../e8f2ff.md>);
  --cl-blue-200:		[BFDBFE](<../BFDBFE.md>);
  --cl-yellow-200:		[FDE68A](<../FDE68A.md>);
  --cl-red-500: 		[fe3c30](<../fe3c30.md>);
  --cl-orange-500:	 	[fe9500](<../fe9500.md>);
  --cl-yellow-500: 		[fecc00](<../fecc00.md>);
  --cl-green-500: 		[27cd41](<../27cd41.md>);
  --cl-blue-500: 		[007aff](<../007aff.md>);
  --cl-indigo-500: 		[5756d5](<../5756d5.md>);
  --cl-purple-500: 		[af52de](<../af52de.md>);
  --cl-pink-500: 		[fe2e55](<../fe2e55.md>);	
  --cl-brown-500: 		[a2845e](<../a2845e.md>);
  --cl-beige-200:		[eec170](<../eec170.md>);
  --cl-beige-500:		[c8963e](<../c8963e.md>);
  --cl-beige-700:		[472515](<../472515.md>);
}```
                - Togetic
                    - ```css
:root {
/*Togetic [176](<../176.md>)*/
  --cl-togetic-gray-500:  [737b83](<../737b83.md>);
  --cl-togetic-gray-300:  [acc5bd](<../acc5bd.md>);
  --cl-togetic-gray-100:  [d5eeee](<../d5eeee.md>);
  --cl-togetic-red-500:   [bd1808](<../bd1808.md>);
  --cl-togetic-red-300:   [de4139](<../de4139.md>);
  --cl-togetic-blue-500:  [1062bd](<../1062bd.md>);
  --cl-togetic-blue-300:  [2994e6](<../2994e6.md>);
}```
                - Wobbufet
                    - ```css
:root {
  /* CSS HEX */
  --uranian-blue: [a4deffff](<../a4deffff.md>);
  --aero: [73bdf6ff](<../73bdf6ff.md>);
  --blue-jeans: [52aceeff](<../52aceeff.md>);
  --yale-blue: [20528bff](<../20528bff.md>);
  --gray-web: [838383ff](<../838383ff.md>);
  --davys-grey: [525252ff](<../525252ff.md>);
  --dark-orange: [ff8b00ff](<../ff8b00ff.md>);
  --persimmon: [de5200ff](<../de5200ff.md>);
  --rufous: [a41000ff](<../a41000ff.md>);
}```
            - UI
                - All Pages
                    - > Modifies the "All Pages" site, found in the left sidebar
                    - Colors
                        - ```css
:root {
  --fg-all-pages-title:					var(--cl-gray-800);
  --bg-all-pages-header:				var(--cl-gray-100);
  --fg-all-pages-header:				var(--cl-gray-800);
  --fg-all-pages-header-sorted:			var(--cl-gray-900);
  --bg-all-pages-clickable-pill:		var(--cl-gray-800);
  --bg-all-pages-search:				var(--cl-white);
  --fg-all-pages-search:				var(--cl-gray-500);
  --fg-all-pages-search-placeholder:	var(--cl-gray-500);
  --fg-all-pages-title-col:				var(--cl-gray-500);
  --fg-all-pages-row:					var(--cl-gray-500);
  --br-all-pages-row:					var(--cl-gray-400);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-all-pages-title:					var(--cl-gray-800);
  --bg-all-pages-header:				var(--cl-gray-100);
  --fg-all-pages-header:				var(--cl-gray-800);
  --fg-all-pages-header-sorted:			var(--cl-gray-900);
  --bg-all-pages-clickable-pill:		var(--cl-gray-800);
  --bg-all-pages-search:				var(--cl-white);
  --fg-all-pages-search:				var(--cl-gray-500);
  --fg-all-pages-search-placeholder:	var(--cl-gray-500);
  --fg-all-pages-title-col:				var(--cl-gray-500);
  --fg-all-pages-row:					var(--cl-gray-500);
  --br-all-pages-row:					var(--cl-gray-400);  
  } 
}```
                - Brackets
                    - > Modifies the color of the Brackets when linking Pages
                    - Colors
                        - ```css
:root {
  --fg-brackets: var(--cl-gray-500);
}

@media (prefers-color-scheme: dark) {
  :root { 
    --fg-brackets: var(--cl-gray-500);
  } 
}```
                - Buttons and Icons 
                    - > Modifies icons in the top- and sidebar as well as buttons in the filter dialog.
                    - Colors
                        - ```css
:root {
  --fg-buttons:			var(--cl-gray-400);
  --bg-buttons: 		transparent;
  --fg-buttons-hover:	var(--cl-gray-500);
  --bg-buttons-hover:	transparent;
  --bg-word-count:		var(--cl-gray-100);
  --fg-word-count:		var(--cl-gray-700);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-buttons:			var(--cl-gray-400);
  --bg-buttons: 		transparent;
  --fg-buttons-hover:	var(--cl-gray-500);
  --bg-buttons-hover:	transparent;
  --bg-word-count:		var(--cl-gray-700);
  --fg-word-count:		var(--cl-gray-100);
  } 
}```
                - Caret
                    - > Modifies the little caret the folds bullets
                    - Colors
                        - ```css
:root {
  --fg-caret: 	var(--cl-gray-500);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-caret: 	var(--cl-gray-300);
  } 
}```
                - Help
                    - > Modifies the help dialog
                    - Colors
                        - ```css
:root {
  --bg-help:	var(--cl-gray-100);
  --fg-help:	var(--cl-gray-600);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-help:	var(--cl-gray-800);
  --fg-help:	var(--cl-gray-400);
  } 
}```
                - Left Sidebar
                    - > Modifies the left sidebar
                    - Colors
                        - ```css
:root {
  --bg-left-sidebar:		var(--cl-gray-50);
  --bg-left-sidebar-hover:	var(--cl-gray-50);
  --bg-left-sidebar-hr:		var(--cl-gray-500);
  --fg-left-sidebar:		var(--cl-gray-700);
  --fg-left-sidebar-hover:	var(--cl-gray-700);
  --fg-left-dropdown-title:	var(--cl-gray-400);
  --fg-left-sidebar-icons: 	var(--cl-gray-500);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-left-sidebar:		var(--cl-gray-800);
  --bg-left-sidebar-hover:	var(--cl-gray-800);
  --bg-left-sidebar-hr:		var(--cl-gray-500);
  --fg-left-sidebar:		var(--cl-gray-100);
  --fg-left-sidebar-hover:	var(--cl-white);
  --fg-left-dropdown-title:	var(--cl-gray-400);
  --fg-left-sidebar-icons: 	var(--cl-gray-400); 
  } 
}```
                - Log
                    - > Modifies the color of the daily log
                    - Colors
                        - ```css
:root {
  --fg-log-hr: 	var(--cl-gray-400);
  --fg-log:		var(--cl-gray-400);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-log-hr: 	var(--cl-gray-600);
  --fg-log:		var(--cl-gray-600);
  } 
}```
                - Menus
                    - > Changes the color and fonts of the different menus

**Notice**
We can't change the selection background in some menus yet, so make sure, that your colors will fit - avoid too light and too dark shades.
                    - Colors
                        - ```css
:root {
  --bg-menu:		var(--cl-white);
  --bg-menu-hover:	var(--cl-gray-100);
  --fg-menu:		var(--cl-gray-500);
  --fg-menu-hover:	var(--cl-gray-600);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-menu:		var(--cl-gray-800);
  --bg-menu-hover:	var(--cl-gray-200);
  --fg-menu:		var(--cl-gray-500);
  --fg-menu-hover:	var(--cl-gray-500);
  } 
}```
                - Top Bar
                    - > Modifies colors and fonts of the topbar including the  "Find or Create Page"-Input.
                    - Colors
                        - ```css
:root {
  --bg-topbar: 				var(--cl-white);
  --bg-input: 				var(--cl-gray-50);
  --br-input: 				var(--cl-gray-100);
  --fg-input: 				var(--cl-gray-800);
  --fg-input-placeholder: 	var(--cl-gray-400);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-topbar: 				var(--cl-gray-900);
  --bg-input: 				var(--cl-gray-800);
  --br-input: 				var(--cl-gray-700);
  --fg-input: 				var(--cl-gray-100);
  --fg-input-placeholder: 	var(--cl-gray-400);
  } 
}```
                - In-Line References
                    - ```css
:root {
	--bg-inline-refs: 	var(--cl-gray-50);
}

@media (prefers-color-scheme: dark) {
  :root { 
	--bg-inline-refs: 	var(--cl-gray-600);
  } 
}```
            - Content
                - Body
                    - ```css
:root {
  --primary-color: 		var(--cl-gray-800);
  --background-color: 	var(--cl-white);
  --bg-body:			var(--cl-white);
  --fg-body:			var(--cl-gray-800);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --primary-color: 		var(--cl-blue-500);
  --background-color: 	var(--cl-gray-900);
  --bg-body:			var(--cl-gray-900);
  --fg-body:			var(--cl-gray-50);

  } 
}```
                - Breadcrumbs
                    - > Modifies the breadcrumbs (zoom items) 
                    - ```css
:root {
  --bg-zoom:			transparent;
  --fg-zoom:			var(--cl-gray-500);
  --bg-zoom-mask:		var(--cl-white);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-zoom:			transparent;
  --fg-zoom:			var(--cl-gray-500);
  --bg-zoom-mask:		var(--cl-gray-50);

  } 
}```
                - Bullets and Lines
                    - > Changes the bullets and lines for blocks
                    - Preview
                        - A single bullet
                            - A line to the left
                        - A closed bullet
                            - 
                    - ```css
:root {
  --bg-bullet-inner:	var(--cl-gray-200);
  --br-bullet-outer:	var(--cl-gray-200);
  --br-block:			var(--cl-gray-200);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-bullet-inner:	var(--cl-gray-700);
  --br-bullet-outer:	var(--cl-gray-500);
  --br-block:			var(--cl-gray-600);
  } 
}```
                - Headings
                    - > Modifies the Headings Level 1 - 3
                    - Preview
                        - Heading 1
                            - Heading 2
                                - Heading 3
                    - ```css
:root {
  --fg-h1:				var(--cl-gray-900);
  --fg-h2:				var(--cl-gray-900);
  --fg-h3:				var(--cl-gray-900);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-h1:				var(--cl-gray-50);
  --fg-h2:				var(--cl-gray-50);
  --fg-h3:				var(--cl-gray-50);
  } 
}```
                - Highlights
                    - > Modifies the highlights
                    - Preview
                        - ^^This text is highlighted^^
                    - Colors
                        - ```css
:root {
  --bg-highlight:		var(--cl-blue-50);
  --bg-highlight-blue:	var(--cl-blue-200);
  --bg-highlight-yellow:var(--cl-blue-200);
  --bg-highlight-grey:	var(--cl-gray-200);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-highlight:		var(--cl-beige-500);
  --bg-highlight-blue:	var(--cl-blue-500);
  --bg-highlight-yellow:var(--cl-blue-500);
  --bg-highlight-grey:	var(--cl-gray-500);
  } 
}```
                - Page Reference Links
                    - > Modifies the color of links and references pages
                    - Preview
                        - This is [a link](http://link.com), this is a reference to a page [Test Page](<../Test Page.md>), this is a [Project/Complete Job Search & Get Hired](<../Project/Complete Job Search & Get Hired.md>) namespace, this is a double underline [[[R:](<../[[R:.md>) Remote Work (podcasts)]]
                    - Colors
                        - ```css
:root {
  --fg-link:						var(--cl-green-500);
  --fg-link-hover:					var(--cl-green-500);
  --fg-reference:					var(--cl-togetic-blue-500);
  --fg-reference-hover:				var(--cl-togetic-blue-300);
  --fg-namespace:					var(--cl-togetic-red-300);
  --fg-namespace-hover:				var(--cl-togetic-red-500);
  --fg-reference-underline:			var(--cl-togetic-gray-300);
  --fg-reference-underline-hover:	var(--cl-togetic-blue-500);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-link:						var(--cl-togetic-blue-300);
  --fg-link-hover:					var(--cl-blue-500);
  --fg-reference:					var(--cl-togetic-red-300);
  --fg-reference-hover:				var(--cl-togetic-red-500);
  --fg-namespace:					var(--cl-orange-500);
  --fg-namespace-hover:				var(--cl-orange-500); 
  --fg-reference-underline:			var(--cl-gray-300);
  --fg-reference-underline-hover:	var(--cl-orange-500);
  } 
}```
                - Block References
                    - > Modifies the background of the reference blocks
                    - Preview
                        - ((IeFN6yma5))
                    - Colors
                        - ```css
:root {
  --bg-reference:				var(--cl-gray-50);
  --bg-block-ref:				none;
  --bg-block-ref-hover: 		none;
  --fg-block-ref-underline:		var(--cl-gray-100);
  --fg-block-ref-start:			var(--cl-orange-500);
  --fg-block-ref-end:			var(--cl-indigo-500);
}

@media (prefers-color-scheme: dark) {
  :root {
  --bg-reference:				var(--cl-gray-800);
  --bg-block-ref:				none;
  --bg-block-ref-hover: 		none;
  --fg-block-ref-underline:		var(--cl-gray-100);
  --fg-block-ref-start:			var(--cl-orange-500);
  --fg-block-ref-end:			var(--cl-gray-50);
  }
}```
                - Tags
                    - > Modifies the apperance of tags
                    - Preview
                        - [tag1](<../tag1.md>) [tag2](<../tag2.md>)
                    - Colors
                        - ```css
:root {
  --fg-tag:				var(--cl-gray-500);
  --bg-tag:				none;
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-tag:				var(--cl-gray-500);
  --bg-tag:				none;
  } 
}```
            - Special Blocks
                - Calc
                    - > Modifies the color of the calculation result
                    - Preview
                        - {{[calc](<../calc.md>): 31 + 11}}
                    - Colors
                        - ```css
:root {
  --fg-calc:		var(--cl-green-500);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-calc:		var(--cl-green-500);
  } 
}```
                - Code
                    - > Modifies the color of Codeblocks and Inline Code
                    - Preview
                        - `Inline code` and Codeblocks:
                            - ```javascript
const baseValue = prompt('Enter the base of a triangle: ');
const heightValue = prompt('Enter the height of a triangle: ');

// calculate the area
const areaValue = (baseValue * heightValue) / 2;

console.log(
  `The area of the triangle is ${areaValue}`
);```
                    - Inline Code
                        - Colors
                            - ```css
:root {
  --fg-inline-code:			var(--cl-gray-800);
  --bg-inline-code:			var(--cl-gray-50);
  --br-inline-code:			var(--cl-gray-50);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --fg-inline-code:			var(--cl-gray-50);
  --bg-inline-code:			var(--cl-gray-700);
  --br-inline-code:			var(--cl-gray-700);  
  } 
}```
                    - Code Block
                        - Colors - Light
                            - ```css
:root {
  --bg-code:						var(--cl-gray-50);
  --bg-code-filler:					var(--cl-gray-50);
  --bg-code-gutters:				var(--cl-gray-50);
  --bg-code-selected:				var(--cl-gray-300);
  --bg-code-selection:				var(--cl-blue-200);
  --bg-code-focused:				var(--cl-blue-200);
  --bg-code-searching:				rgba(255, 255, 0, 0.4);	
  --bg-code-matchingtag:			rgba(255, 150, 0, 0.3);
  --bg-code-activeline:				var(--cl-white);
  --bg-code-fat-cursor:				[7e7](<../7e7.md>);
  --bg-code-fat-cursor-mark:		rgba(20, 255, 20, 0.5);
  --bg-code-fat-cursor-animate:		[7e7](<../7e7.md>);
  --br-code-gutters:				var(--cl-gray-100);
  --br-code-cursor:					var(--cl-black);
  --br-code-secondary-cursor:		var(--cl-gray-400);
  --br-code-ruler:					var(--cl-gray-400);
  --fg-code-linenumber:				var(--cl-gray-500);
  --fg-code-guttermarker:			var(--cl-black);
  --fg-code-guttermarker-subtle: 	var(--cl-gray-500);
}```
                        - Colors - Dark
                            - ```css
@media (prefers-color-scheme: dark) {
  :root { 
  --bg-code:						var(--cl-gray-800);
  --bg-code-filler:					var(--cl-gray-800);
  --bg-code-gutters:				var(--cl-gray-800);
  --bg-code-selected:				var(--cl-gray-300);
  --bg-code-selection:				var(--cl-blue-200);
  --bg-code-focused:				var(--cl-blue-200);
  --bg-code-searching:				rgba(255, 255, 0, 0.4);	
  --bg-code-matchingtag:			rgba(255, 150, 0, 0.3);
  --bg-code-activeline:				var(--cl-white);
  --bg-code-fat-cursor:				[7e7](<../7e7.md>);
  --bg-code-fat-cursor-mark:		rgba(20, 255, 20, 0.5);
  --bg-code-fat-cursor-animate:		[7e7](<../7e7.md>);
  --br-code-gutters:				var(--cl-gray-900);
  --br-code-cursor:					var(--cl-white);
  --br-code-secondary-cursor:		var(--cl-gray-600);
  --br-code-ruler:					var(--cl-gray-600);
  --fg-code-linenumber:				var(--cl-gray-500);
  --fg-code-guttermarker:			var(--cl-black);
  --fg-code-guttermarker-subtle: 	var(--cl-gray-500);
  } 
}```
                    - Syntax Highlighting
                        - Colors - Light
                            - ```css
:root {  
  --fg-code:					var(--cl-gray-400);
  --fg-code-header:				var(--cl-blue-500);
  --fg-code-quote:				var(--cl-green-500);
  --fg-code-negative:			var(--cl-green-500);
  --fg-code-positive:			var(--cl-green-500);
  --fg-code-keyword:			var(--cl-purple-500);
  --fg-code-atom:				var(--cl-blue-500);
  --fg-code-number:				var(--cl-green-500);
  --fg-code-def:				var(--cl-blue-500);
  --fg-code-variable-2:			var(--cl-indigo-500);
  --fg-code-variable-3:			var(--cl-green-500);
  --fg-code-comment:			var(--cl-brown-500);
  --fg-code-string:				var(--cl-green-500);
  --fg-code-string-2:			var(--cl-orange-500);
  --fg-code-meta:				var(--cl-gray-400);
  --fg-code-qualifier:			var(--cl-gray-400);
  --fg-code-builtin:			var(--cl-indigo-500);
  --fg-code-bracket:			var(--cl-gray-500);
  --fg-code-tag:				var(--cl-green-500);
  --fg-code-attribute:			var(--cl-blue-500);
  --fg-code-hr:					var(--cl-gray-600);
  --fg-code-link:				var(--cl-blue-500);
  --fg-code-error:				var(--cl-green-500);
  --fg-code-invalidchar:		var(--cl-green-500);
  --fg-code-matchingbracket: 	var(--cl-green-500);
  --fg-code-nonmatchingbracket:	var(--cl-green-500);
}```
                        - Colors - Dark
                            - ```css
@media (prefers-color-scheme: dark) {
  :root { 
  --fg-code:					var(--cl-gray-300);
  --fg-code-header:				var(--cl-blue-500);
  --fg-code-quote:				var(--cl-green-500);
  --fg-code-negative:			var(--cl-green-500);
  --fg-code-positive:			var(--cl-green-500);
  --fg-code-keyword:			var(--cl-purple-500);
  --fg-code-atom:				var(--cl-blue-500);
  --fg-code-number:				var(--cl-green-500);
  --fg-code-def:				var(--cl-blue-500);
  --fg-code-variable-2:			var(--cl-indigo-500);
  --fg-code-variable-3:			var(--cl-green-500);
  --fg-code-comment:			var(--cl-brown-500);
  --fg-code-string:				var(--cl-green-500);
  --fg-code-string-2:			var(--cl-orange-500);
  --fg-code-meta:				var(--cl-gray-400);
  --fg-code-qualifier:			var(--cl-gray-400);
  --fg-code-builtin:			var(--cl-indigo-500);
  --fg-code-bracket:			var(--cl-gray-500);
  --fg-code-tag:				var(--cl-green-500);
  --fg-code-attribute:			var(--cl-blue-500);
  --fg-code-hr:					var(--cl-gray-600);
  --fg-code-link:				var(--cl-blue-500);
  --fg-code-error:				var(--cl-green-500);
  --fg-code-invalidchar:		var(--cl-green-500);
  --fg-code-matchingbracket: 	var(--cl-green-500);
  --fg-code-nonmatchingbracket:	var(--cl-green-500);  
  } 
}```
                - Diagrams
                    - > Diagrams can't be modified yet. This is a problem with dark mode settings. 
                    - Preview
                        - {{[diagram](<../diagram.md>)}}
                            - A
                            - B
                - Embed
                    - > Changes the background color of embed blocks
                    - Preview
                        - Sample Data
                            - Embed 1
                                - {{[embed](<../embed.md>): ((ZuyIjM6mE))}}
                            - Embed 2
                                - {{[embed](<../embed.md>): ((oVEJn3mnp))}}
                            - Embed 3
                        - {{[embed](<../embed.md>): ((CR-dOUiRZ))}}
                    - Colors
                        - ```css
:root {
  --bg-embed-1: 	var(--cl-gray-50);
  --bg-embed-2: 	var(--cl-gray-100);
  --bg-embed-3: 	var(--cl-gray-200);
  --bg-embed-4: 	var(--cl-gray-300);
  --bg-embed-5: 	var(--cl-gray-400);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-embed-1: 	var(--cl-gray-800);
  --bg-embed-2: 	var(--cl-gray-700);
  --bg-embed-3: 	var(--cl-gray-600);
  --bg-embed-4: 	var(--cl-gray-500);
  --bg-embed-5: 	var(--cl-gray-400);  
  } 
}```
                - HR
                    - > Modifies horizontal lines
                    - Preview
                        - ---
                    - Colors
                        - ```css
:root {
 --br-hr:	var(--cl-gray-300);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --br-hr:	var(--cl-gray-300);
  } 
}```
                - Kanban
                    - > Modifies Kanban boards
                    - Preview
                        - {{[kanban](<../kanban.md>)}}
                            - Ready
                                - Card 1
                            - Done
                                - Card 2
                    - Colors
                        - ```css
:root {
  --bg-kanban-board: 	var(--cl-gray-50);
  --br-kanban-board:	var(--cl-white);
  --bg-kanban-column:	var(--cl-gray-100);
  --bg-kanban-card:		var(--cl-white);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-kanban-board: 	var(--cl-gray-800);
  --br-kanban-board:	var(--cl-black);
  --bg-kanban-column:	var(--cl-gray-900);
  --bg-kanban-card:		var(--cl-black);  
  } 
}```
                - Mermaid
                    - > Modifies Mermaid diagrams
                    - Preview
                        - {{mermaid}}
                            - graph TD;
                                - A-->B;
                                - A-->D;
                                - B-->D;
                                - C-->D;
                    - Colors
                        - ```css
:root {
  --bg-mermaid: 		var(--cl-white);
  --bg-mermaid-node: 	var(--cl-gray-300);
  --fg-mermaid-label: 	var(--cl-gray-800);
  --br-mermaid-node: 	var(--cl-gray-500);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-mermaid: 		var(--cl-white);
  --bg-mermaid-node: 	var(--cl-gray-300);
  --fg-mermaid-label: 	var(--cl-gray-800);
  --br-mermaid-node: 	var(--cl-gray-500);  
  } 
}```
                - Queries
                    - > Modifies the appearance of queries
                    - Preview
                        - {{[query](<../query.md>): {and: [TODO](<../TODO.md>) [December 30th, 2020](<../December 30th, 2020.md>)}}}
                    - Colors
                        - ```css
:root {
  --bg-query-title:		var(--cl-gray-100);
  --fg-query-title:		var(--cl-gray-600);
  --br-query:			var(--cl-gray-200);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-query-title:		var(--cl-gray-900);
  --fg-query-title:		var(--cl-gray-400);
  --br-query:			var(--cl-gray-700);  
  } 
}```
                - Quote
                    - > Modifies the design of quotes
                    - Preview
                        - > This is a famous quote!
                    - Color
                        - ```css
:root {
  --bg-quote:			var(--cl-white);
  --br-quote:			var(--cl-gray-800);
  --fg-quote:			var(--cl-gray-800);  
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-quote:			var(--cl-gray-900);
  --br-quote:			var(--cl-gray-500);
  --fg-quote:			var(--cl-gray-100);    
  } 
}```
                - Tables
                    - > Modifies tables
                    - Preview
                        - {{[table](<../table.md>)}}
                            - Column 1
                                - Column 2
                            - Row 1
                                - Row 2
                    - Colors
                        - ```css
:root {
  --br-table:	var(--cl-gray-300);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --br-table:	var(--cl-gray-600);
  } 
}```
                - Todo
                    - > Modifies the design of todos
                    - Preview
                        - [ ] This is a todo
                        - [x] This is a finished todo
                    - Colors
                        - ```css
:root {
  --br-checkbox: var(--cl-gray-300);
  --bg-checkbox-checked: var(--cl-gray-300);
  --br-checkmark: var(--cl-white);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --br-checkbox: var(--cl-gray-600);
  --bg-checkbox-checked: var(--cl-gray-600);
  --br-checkmark: var(--cl-white);  
  } 
}```
                - Versions
                    - > Modifies the design of the version block
                    - Preview
                        - Version 2
                    - Colors
                        - ```css
:root {
  --bg-version-bullet: 		var(--cl-gray-400);
  --fg-version-selected: 	var(--cl-blue-500);
  --br-version:				var(--cl-gray-300);
}

@media (prefers-color-scheme: dark) {
  :root { 
  --bg-version-bullet: 		var(--cl-gray-600);
  --fg-version-selected: 	var(--cl-blue-500);
  --br-version:				var(--cl-gray-600);  
  } 
}```
            - Custom
                - ((6YHNhSFRA))
                    - ```css
:root {
  --note-tag-color:				var(--cl-gray-700);
}

@media (prefers-color-scheme: dark) {
  :root {
  	--note-tag-color:			var(--cl-gray-200);
  }
}```
    - ## Styling Elements
        1. Tag Styling [Status](<../Status.md>)/Enabled [Highlights](<../Highlights.md>) [tags](<../tags.md>)
            1. `GTD Tags`
                - `GTD Tags`
                    - `[INBOX](<../INBOX.md>)
[Inbox](<../Inbox.md>)
[Projects](<../Projects.md>)
[Goals](<../Goals.md>)
#[Follow Up](<../Follow Up.md>)
[Mindsweep](<../Mindsweep.md>)
[Waiting](<../Waiting.md>)
#[Waiting-[[resolved](<../Waiting-[[resolved.md>)]]
[Tracking](<../Tracking.md>)
#[Daily Big 3](<../Daily Big 3.md>)
#[Plan My Day](<../Plan My Day.md>)
#[Weekly Preview](<../Weekly Preview.md>)
#[Next Steps](<../Next Steps.md>)
[GTD](<../GTD.md>)
                        - ```css
:root {
  --background:[607D8B](<../607D8B.md>);
  --color:[FFFFFF](<../FFFFFF.md>);
  --padding:2px 5px 2px 5px;
  --font-size: 13px;
  --line-height: 1em;
  --font-weight: 500;
  --border-radius: 5px 5px 5px 5px;
  --position:relative;
  
  
}

span.rm-page-ref[data-tag="GTD"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="GTD"]:before {
    content: '✅'
}

span.rm-page-ref[data-tag="INBOX"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="INBOX"]:before {
    content: '📥'
}

span.rm-page-ref[data-tag="Inbox"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Inbox"]:before {
    content: '📥'
}

span.rm-page-ref[data-tag="Projects"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Projects"]:before {
    content: '🔨'
}

span.rm-page-ref[data-tag="Goals"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Goals"]:before {
    content: '🎯'
}

span.rm-page-ref[data-tag="Follow Up"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Follow Up"]:before {
    content: '📌'
}

span.rm-page-ref[data-tag="Mindsweep"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Mindsweep"]:before {
    content: '🧹'
}

span.rm-page-ref[data-tag="Waiting"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Waiting"]:before {
    content: '⏱'
}

span.rm-page-ref[data-tag="Waiting-[resolved](<../resolved.md>)"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Waiting-[resolved](<../resolved.md>)"]:before {
    content: '☑️'
}

span.rm-page-ref[data-tag="Tracking"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Tracking"]:before {
    content: '👀'
}

span.rm-page-ref[data-tag="Daily Big 3"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Daily Big 3"]:before {
    content: '🚩'
}

span.rm-page-ref[data-tag="Plan My Day"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Plan My Day"]:before {
    content: '🎯'
}

span.rm-page-ref[data-tag="Weekly Preview"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Weekly Preview"]:before {
    content: '🗓'
}

span.rm-page-ref[data-tag="Next Steps"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Next Steps"]:before {
    content: '➡️'
}```
            2. `Zettelkasten Tags`
                - `#[Reference Notes](<../Reference Notes.md>)
                    - ```css
span.rm-page-ref[data-tag="Reference Notes"] {
	background-image: linear-gradient(90deg, [BEDFF8](<../BEDFF8.md>), [BEDFF8](<../BEDFF8.md>), [BEDFF8](<../BEDFF8.md>));
	background-size: 100%;
    color: [000000](<../000000.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - `#[Seedlings](<../Seedlings.md>)
                    - ```css
span.rm-page-ref[data-tag="Seedlings"] {
    color: [FFFFFF](<../FFFFFF.md>) !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: [FFEFBA](<../FFEFBA.md>);  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, [A6DA69](<../A6DA69.md>), [A6DA69](<../A6DA69.md>));  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, [A6DA69](<../A6DA69.md>), [A6DA69](<../A6DA69.md>)); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}




```
                - `[Annotations](<../Annotations.md>)
                    - ```css
span.rm-page-ref[data-tag="Annotations"] {
    background: [795548E2](<../795548E2.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - `#[Fleeting Notes](<../Fleeting Notes.md>)
                    - ```css
span.rm-page-ref[data-tag="Fleeting Notes"] {
    color: [1A1718](<../1A1718.md>) !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: [FFEFBA](<../FFEFBA.md>);  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, [FFEFBA](<../FFEFBA.md>), [FFEFBA](<../FFEFBA.md>));  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, [FFEFBA](<../FFEFBA.md>), [FFEFBA](<../FFEFBA.md>)); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}




```
                - `#[Literature Notes](<../Literature Notes.md>) [Test](<../Test.md>)
                    - ```css
span.rm-page-ref[data-tag="Literature Notes"] {
	background-image: linear-gradient(90deg, [3A98E3](<../3A98E3.md>), [3A98E3](<../3A98E3.md>), [3A98E3](<../3A98E3.md>));
	background-size: 100%;
    color: [FFFFFF](<../FFFFFF.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}



```
                - `#[Evergreen Notes](<../Evergreen Notes.md>) [Test](<../Test.md>)
                    - ```css
span.rm-page-ref[data-tag="Evergreen Notes"] {
	background-image: linear-gradient(90deg, [507B58](<../507B58.md>), [507B58](<../507B58.md>), [507B58](<../507B58.md>));
	background-size: 100%;
    color: [EEF2EE](<../EEF2EE.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

/* span.rm-page-ref[data-tag="Permanent Notes"] + span[data-link-title] {
     background: [DCE5DE8C](<../DCE5DE8C.md>) !important;
     color: [F3F7F2](<../F3F7F2.md>) !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}*/


/*span.rm-page-ref[data-tag="Permanent Notes"]:after, span.rm-page-ref[data-tag="Permanent Notes"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}*/

span.rm-page-ref[data-tag="Permanent Notes"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: [507B58](<../507B58.md>);
    border-width: 10px;
    margin-top: -10px;
}

span.rm-page-ref[data-tag="Permanent Notes"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: [507B58](<../507B58.md>);
    border-width: 10px;
    margin-top: -10px;
}



```
                - `#[Zettel Questions](<../Zettel Questions.md>)
                    ```clojure
span.rm-page-ref[data-tag="Zettel Questions"] {
    color: [FFFFFF](<../FFFFFF.md>) !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: [BC6DCA](<../BC6DCA.md>);  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, [BC6DCA](<../BC6DCA.md>), [BC6DCA](<../BC6DCA.md>));  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, [BC6DCA](<../BC6DCA.md>), [BC6DCA](<../BC6DCA.md>)); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}




```
                - `#[Branching Notes](<../Branching Notes.md>) [Test](<../Test.md>)
                    - ```css
span.rm-page-ref[data-tag="Branching Notes"] {
background: [B79891](<../B79891.md>);  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, [94716B](<../94716B.md>), [94716B](<../94716B.md>));  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, [94716B](<../94716B.md>), [94716B](<../94716B.md>)); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

	background-size: 100%;
    color: [EEF2EE](<../EEF2EE.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

/* span.rm-page-ref[data-tag="Branching Notes"] + span[data-link-title] {
     background: [B7989128](<../B7989128.md>) !important;
     color: [F3F7F2](<../F3F7F2.md>) !important;
     padding: 3px 5px 3px 5px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0px 5px 5px 0px;
     margin-left: -5px;
} */





```
                - `#[Intermediary Notes](<../Intermediary Notes.md>)
                    - ```css
span.rm-page-ref[data-tag="Intermediary Notes"] {
	color: [1A1718](<../1A1718.md>) !important;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: [607D8B68](<../607D8B68.md>);  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, [607D8B68](<../607D8B68.md>), [607D8B68](<../607D8B68.md>));  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, [607D8B68](<../607D8B68.md>), [607D8B68](<../607D8B68.md>)); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

  
}

```
                - `#[Project Ideas](<../Project Ideas.md>)
                    - ```css
span.rm-page-ref[data-tag="Project Ideas"] {
	color: [1A1718](<../1A1718.md>) !important;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: [FF572268](<../FF572268.md>);  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, [FF572268](<../FF572268.md>), [FF572268](<../FF572268.md>));  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, [FF572268](<../FF572268.md>), [FF572268](<../FF572268.md>)); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

  
}

```
                - [Evergreen](<../Evergreen.md>)
                    - Tag
                        - ```css
span.rm-page-ref[data-tag="Evergreen"]:before {
    content: '🌲 '
}

span.rm-page-ref[data-tag="Evergreen"]:after {
    content: ':'
}

span.rm-page-ref[data-tag="Evergreen"] {
 color: var(--note-tag-color) !important;
 padding: 1px 1px !important;
 font-weight: 700 !important;
}```
                    - In Block Reference
                        - Example: "[Evergreen](<../Evergreen.md>) Prefer note titles with complete phrases to sharpen claims"
                        - ```css
.rm-block-ref > span > span.rm-page-ref--tag[data-tag="Evergreen"]{
  /*display: none;*/
  font-size: .1px;
  line-height: 1.5em;
}

.rm-block-ref > span > span.rm-page-ref--tag[data-tag="Evergreen"]:before{
  font-size: 12px;
  margin-right: -5px;
}```
            3. `Areas Tags`
                - `#[Administration](<../Administration.md>)
            4. `Data-type Tags`
                - `[Articles](<../Articles.md>)
                    - ```css
span.rm-page-ref[data-tag="Articles"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Articles"]:before {
    content: '📰'
}```
                - `[Books](<../Books.md>)
                    - ```css
span.rm-page-ref[data-tag="Books"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Books"]:before {
    content: '📚'
}```
                - `[Experiments](<../Experiments.md>)
                    - ```css
span.rm-page-ref[data-tag="Experiments"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Experiments"]:before {
    content: '🧪'
}```
                - `[Tweets](<../Tweets.md>)
                    - ```css
span.rm-page-ref[data-tag="Tweets"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Tweets"]:before {
    content: '🐦'
}```
                - `#[Conversations and Meetings](<../Conversations and Meetings.md>)
                    - ```css
span.rm-page-ref[data-tag="Conversations and Meetings"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Conversations and Meetings"]:before {
    content: '💬'
}```
                - `[Podcasts](<../Podcasts.md>)
                    - ```css
span.rm-page-ref[data-tag="Podcasts"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Podcasts"]:before {
    content: '🎙'
}```
                - `[Meetings](<../Meetings.md>)
                    - ```css
span.rm-page-ref[data-tag="Meetings"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Meetings"]:before {
    content: '👥'
}```
                - `[Conversations](<../Conversations.md>)
                    - ```css
span.rm-page-ref[data-tag="Conversations"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Conversations"]:before {
    content: '🗣'
}```
                - `[Discoveries](<../Discoveries.md>)
                    - ```css
span.rm-page-ref[data-tag="Discoveries"] {
    background: [03A9F4](<../03A9F4.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Discoveries"]:before {
    content: '🎈'
}```
                - `[Lectures](<../Lectures.md>)
                    - ```css
span.rm-page-ref[data-tag="Lectures"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Lectures"]:before {
    content: '🏫'
}```
                - `#[Learning Objectives](<../Learning Objectives.md>)
                    - ```css
span.rm-page-ref[data-tag="Learning Objectives"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Learning Objectives"]:before {
    content: '🎓'
}```
                - `[Recommendations](<../Recommendations.md>)
                    - ```css
span.rm-page-ref[data-tag="Recommendations"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Recommendations"]:before {
    content: '📍'
}```
                - `[Ideas](<../Ideas.md>)
                    - ```css
span.rm-page-ref[data-tag="Ideas"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Ideas"]:before {
    content: '💡'
}```
                - `[Jokes](<../Jokes.md>)
                    - ```css
span.rm-page-ref[data-tag="Jokes"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Jokes"]:before {
    content: '🤣'
}```
                - `[Frameworks](<../Frameworks.md>)
                    - ```css
span.rm-page-ref[data-tag="Frameworks"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Frameworks"]:before {
    content: '⚙️'
}```
                - `#[Goal Ideas](<../Goal Ideas.md>)
                    - ```css
span.rm-page-ref[data-tag="Goal Ideas"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Goal Ideas"]:before {
    content: '🎯'
}```
                - `#[Graph Mentorship](<../Graph Mentorship.md>)
                    - ```css
span.rm-page-ref[data-tag="Graph Mentorship"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Graph Mentorship"]:before {
    content: '🤝'
}```
                - `#[Prompt Ideas](<../Prompt Ideas.md>)
                    - ```css
span.rm-page-ref[data-tag="Prompt Ideas"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Prompt Ideas"]:before {
    content: '💭'
}```
                - `[Quotes](<../Quotes.md>)
                    - ```css
span.rm-page-ref[data-tag="Quotes"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Quotes"]:before {
    content: '💬'
}```
                - `[Prompts](<../Prompts.md>)
                    - ```css
span.rm-page-ref[data-tag="Prompts"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Prompts"]:before {
    content: '💭'
}```
                - `[People](<../People.md>)
                    - ```css
span.rm-page-ref[data-tag="People"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="People"]:before {
    content: '😃'
}```
                - `[Members](<../Members.md>)
                    - ```css
span.rm-page-ref[data-tag="Members"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Members"]:before {
    content: '🔑'
}```
                - `[Observations](<../Observations.md>)
                    - ```css
span.rm-page-ref[data-tag="Observations"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Observations"]:before {
    content: '👀'
}```
                - `[Opportunities](<../Opportunities.md>)
                    - ```css
span.rm-page-ref[data-tag="Opportunities"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Opportunities"]:before {
    content: '🚀'
}```
                - `[Examples](<../Examples.md>)
                    - ```css
span.rm-page-ref[data-tag="Examples"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Examples"]:before {
    content: '🏷'
}```
                - `[Transcript](<../Transcript.md>)
                    - ```css
span.rm-page-ref[data-tag="Transcript"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Transcript"]:before {
    content: '📜'
}```
                - `[missing-list](<../missing-list.md>)
                    - ```css
span.rm-page-ref[data-tag="missing-list"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="missing-list"]:before {
    content: '🔍'
}```
                - `[Conventions](<../Conventions.md>)
                    - ```css
span.rm-page-ref[data-tag="Conventions"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Conventions"]:before {
    content: '⚙️'
}```
                - `[Processes](<../Processes.md>)
                    - ```css
span.rm-page-ref[data-tag="Processes"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Processes"]:before {
    content: '⚙️'
}```
                - `[Resources](<../Resources.md>)
                    - ```css
span.rm-page-ref[data-tag="Resources"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Resources"]:before {
    content: '🗃'
}```
                - `[Stories](<../Stories.md>)
                    - ```css
span.rm-page-ref[data-tag="Stories"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Stories"]:before {
    content: '🎭'
}```
                - `[Sprints](<../Sprints.md>)
                    - ```css
span.rm-page-ref[data-tag="Sprints"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Sprints"]:before {
    content: '🏃‍♂️'
}```
                - `[Predictions](<../Predictions.md>)
                    - ```css
span.rm-page-ref[data-tag="Predictions"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Predictions"]:before {
    content: '🔮'
}```
                - `[Replies](<../Replies.md>)
                    - ```css
span.rm-page-ref[data-tag="Replies"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Replies"]:before {
    content: '💬'
}```
                - `[Idioms](<../Idioms.md>)
                    - ```css
span.rm-page-ref[data-tag="Idioms"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Idioms"]:before {
    content: '🗣'
}```
                - `[Timestamps](<../Timestamps.md>)
                    - ```css
span.rm-page-ref[data-tag="Timestamps"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - `[Tips](<../Tips.md>)
                    - ```css
span.rm-page-ref[data-tag="Tips"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Tips"]:before {
    content: '☝️'
}```
                - `[Tensions](<../Tensions.md>)
                    - ```css
span.rm-page-ref[data-tag="Tensions"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Tensions"]:before {
    content: '⛓'
}```
                - `[Templates](<../Templates.md>)
                    - ```css
span.rm-page-ref[data-tag="Templates"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Templates"]:before {
    content: '📄'
}```
                - `#[Q](<../Q.md>)
                    - ```clojure
span.rm-page-ref[data-tag="Context Questions"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Context Questions"]:before {
    content: '❓'
}```
                - `#[Open Questions](<../Open Questions.md>)
                    - ```clojure
span.rm-page-ref[data-tag="Open Questions"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Open Questions"]:before {
    content: '❓'
}```
                - `[Q](<../Q.md>)
                    - ```css
span.rm-page-ref[data-tag="Q"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Q"]:before {
    content: '❓'
}```
                - `[Shownotes](<../Shownotes.md>)
                    - ```css
span.rm-page-ref[data-tag="Shownotes"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - `#[Weather Report](<../Weather Report.md>)
                    - ```css
span.rm-page-ref[data-tag="Weather Report"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Weather Report"]:before {
    content: '🌤'
}```
            5. `Collaboration Tags`
                - `#[Tips & Tricks](<../Tips & Tricks.md>)
                    - ```css
span.rm-page-ref[data-tag="Tips & Tricks"] {
    background: [4CAF50](<../4CAF50.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Tips & Tricks"]:before {
    content: '🔑'
}```
                - `[Questions](<../Questions.md>)
                    - ```css
span.rm-page-ref[data-tag="Questions"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Questions"]:before {
    content: '❓'
}```
                - [Reply-from](<../Reply-from.md>) [Your Name](<../Your Name.md>)
                    - ```css
span.rm-page-ref[data-tag="Reply-from"] {
	background-image: linear-gradient(to right, [CD4CE3AD](<../CD4CE3AD.md>),[CD4CE3AD](<../CD4CE3AD.md>));
	background-size: 100%;
    color: rgb(255,255,255);
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    font-weight: 500;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Reply-from"] + span[data-link-title] {
     background: [e4ffe3](<../e4ffe3.md>) !important;
     color: [F3F7F2](<../F3F7F2.md>) !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Reply-from"]:after, span.rm-page-ref[data-tag="Question"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Reply-from"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: [CD4CE3AD](<../CD4CE3AD.md>);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Reply-from"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: [CD4CE3AD](<../CD4CE3AD.md>);
    border-width: 11px;
    margin-top: -11px;
}


```
                - `[Conversation](<../Conversation.md>)
                    - ```css
span.rm-page-ref[data-tag="Conversation"] {
    background: [9C27B0](<../9C27B0.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Conversation"]:before {
    content: '💬'
}```
                - `[Announcements](<../Announcements.md>)
                    - ```css
span.rm-page-ref[data-tag="Announcements"] {
    background: [F44336](<../F44336.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Announcements"]:before {
    content: '📢'
}```
                - `#[Change Log](<../Change Log.md>)
                    - ```css
span.rm-page-ref[data-tag="Change Log"] {
    background: [4CAF50](<../4CAF50.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Change Log"]:before {
    content: '📢'
}```
                - `[Promptstorming](<../Promptstorming.md>)
                    - ```css
span.rm-page-ref[data-tag="Promptstorming"] {
    background: [98160C](<../98160C.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Promptstorming"]:before {
    content: '🌪️'
}```
                - `#[Help Wanted](<../Help Wanted.md>)
                    - ```css
span.rm-page-ref[data-tag="Help Wanted"] {
    background: [9C27B0](<../9C27B0.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Help Wanted"]:before {
    content: '😃'
}```
                - `#[Dice Roll](<../Dice Roll.md>)
                    - ```css
span.rm-page-ref[data-tag="Dice Roll"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Dice Roll"]:before {
    content: '🎲'
}```
                - `#[Scratchpad](<../Scratchpad.md>)
                    - ```css
span.rm-page-ref[data-tag="Scratchpad"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Scratchpad"]:before {
    content: '✏️'
}```
                - `#[Bookmarks](<../Bookmarks.md>)
                    - ```css
span.rm-page-ref[data-tag="Bookmarks"] {
    background: [2196F3](<../2196F3.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Bookmarks"]:before {
    content: '💾'
}```
                - `#[The Main Feed](<../The Main Feed.md>)
                    - ```css
span.rm-page-ref[data-tag="The Main Feed"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="The Main Feed"]:before {
    content: '⭐️'
}```
                - `#[Daily Log](<../Daily Log.md>)
                    - ```css
span.rm-page-ref[data-tag="Daily Log"] {
    background: [FF9800](<../FF9800.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Daily Log"]:before {
    content: '📆'
}```
                - `#[Daily Activities](<../Daily Activities.md>)
                    - ```css
span.rm-page-ref[data-tag="Daily Activities"] {
    background: [4CAF50](<../4CAF50.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Daily Activities"]:before {
    content: '✍🏼'
}```
                - #[My Daily Notes](<../My Daily Notes.md>) [Your Name](<../Your Name.md>)
                    - ```css
span.rm-page-ref[data-tag="My Daily Notes"] {
	background-image: linear-gradient(to right, [607D8B](<../607D8B.md>),[607D8B](<../607D8B.md>));
	background-size: 100%;
    color: rgb(255,255,255);
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="My Daily Notes"] + span[data-link-title] {
     background: [e4ffe3](<../e4ffe3.md>) !important;
     color: [F3F7F2](<../F3F7F2.md>) !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="My Daily Notes"]:after, span.rm-page-ref[data-tag="Post"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="My Daily Notes"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: [607D8B](<../607D8B.md>);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="My Daily Notes"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: [607D8B](<../607D8B.md>);
    border-width: 11px;
    margin-top: -11px;
}```
                - #[Posted by](<../Posted by.md>) [Your Name](<../Your Name.md>)
                - `#[Chat](<../Chat.md>)
                    - ```css
span.rm-page-ref[data-tag="Chat"] {
    background: [2196F3](<../2196F3.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Chat"]:before {
    content: '📢'
}```
                - `[Chat](<../Chat.md>) [Your Name](<../Your Name.md>) #@ [Beau Haan 📌](<../Beau Haan 📌.md>)`
                    - ```ruby
span.rm-page-ref[data-tag="Chat"] {
	background-image: linear-gradient(to right, [4c8dc9](<../4c8dc9.md>),[4c8dc9](<../4c8dc9.md>));
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
 
}

/* span.rm-page-ref[data-tag="Chat"] + span[data-link-title] {
     background: [e4ffe3](<../e4ffe3.md>) !important;
     color: [F3F7F2](<../F3F7F2.md>) !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Chat"]:after, 
span.rm-page-ref[data-tag="Chat"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Chat"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: [4c8dc9](<../4c8dc9.md>);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Chat"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: [4c8dc9](<../4c8dc9.md>);
    border-width: 11px;
    margin-top: -11px;
}
*/
```
                - [Reply](<../Reply.md>)
                    - ```css
span.rm-page-ref[data-tag="Reply"] {
	background: [CD4CE3AD](<../CD4CE3AD.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}
  
/* span.rm-page-ref[data-tag="Reply"] + span[data-link-title] {
     background: [e4ffe3](<../e4ffe3.md>) !important;
     color: [F3F7F2](<../F3F7F2.md>) !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Reply"]:after, span.rm-page-ref[data-tag="Reply"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Reply"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: [CD4CE3AD](<../CD4CE3AD.md>);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Reply"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: [CD4CE3AD](<../CD4CE3AD.md>);
    border-width: 11px;
    margin-top: -11px;
}
*/
```
                - [Question](<../Question.md>) [Their Name](<../Their Name.md>)
                - [Help](<../Help.md>) [Your Name](<../Your Name.md>)
                    - ```css
span.rm-page-ref[data-tag="Help"] {
	background-image: linear-gradient(to right, [FF9800](<../FF9800.md>),[FF9800](<../FF9800.md>));
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Help"] + span[data-link-title] {
     background: [e4ffe3](<../e4ffe3.md>) !important;
     color: [F3F7F2](<../F3F7F2.md>) !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Help"]:after, span.rm-page-ref[data-tag="Help"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Help"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: [FF9800](<../FF9800.md>);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Help"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: [FF9800](<../FF9800.md>);
    border-width: 11px;
    margin-top: -11px;
}



```
                - #@ [Their Name](<../Their Name.md>)
                    - ```css
span.rm-page-ref[data-tag="@"] {
	background-image: linear-gradient(to right, [4c8dc9](<../4c8dc9.md>),[4c8dc9](<../4c8dc9.md>));
	background-size: 100%;
    color: [EEF2EE](<../EEF2EE.md>);
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="@"] + span[data-link-title] {
     background: [e4ffe3](<../e4ffe3.md>) !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="@"]:after, span.rm-page-ref[data-tag="@"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="@"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: [4c8dc9](<../4c8dc9.md>);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="@"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: [4c8dc9](<../4c8dc9.md>);
    border-width: 11px;
    margin-top: -11px;
}




```
                - [Polls](<../Polls.md>)
                    - ```css
span.rm-page-ref[data-tag="Polls"] {
    color: white !important;
    padding: 3px 5px 3px 5px;
	font-size: 13px;
    line-height: 1em;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: [FFEFBA](<../FFEFBA.md>);  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, [FFFFFF](<../FFFFFF.md>), [FFEFBA](<../FFEFBA.md>));  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, [5856d6](<../5856d6.md>), [5856d6](<../5856d6.md>)); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}






```
                - [Video](<../Video.md>)
                    - ```css
span.rm-page-ref[data-tag="Video"] {
	background-image: linear-gradient(to right, [0D71EB](<../0D71EB.md>),[0D71EB](<../0D71EB.md>));
	background-size: 100%;
    color: white;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Video"] + span[data-link-title] {
     background: white !important;
     padding: 2px 5px 2px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border: 1px solid [0D71EB](<../0D71EB.md>);
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Video"]:after, span.rm-page-ref[data-tag="Video"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Video"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: [0D71EB](<../0D71EB.md>);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Video"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: [0D71EB](<../0D71EB.md>);
    border-width: 11px;
    margin-top: -11px;
}




```
                - Notifications & Mentions:
                    - **[Example](<../Example.md>):**
                        - [@[[Their Name](<../@[[Their Name.md>)]]
                        - [cc:[[Their Name](<../cc:[[Their Name.md>)]]
                        - [~[[Your Name](<../~[[Your Name.md>)]]
                        - [^[[Your Name](<../^[[Your Name.md>)]]
                    - ```css
span[data-link-title^="@"] {
        border: 2px solid [a76800](<../a76800.md>) !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="@"]:before {
    color: [000746](<../000746.md>) !important;
    content: "🚨unread "
}

span[data-link-title^="~"] {
        border: 2px solid [02B920](<../02B920.md>) !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="~"]:before {
    color: [000746](<../000746.md>) !important;
    content: "✅read "
}

span[data-link-title^="^"] {
        border: 2px solid [4CAF50](<../4CAF50.md>) !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="^"]:before {
    color: [000746](<../000746.md>) !important;
    content: "💾saved "
}

span[data-link-title^="cc:"] {
        border: 2px solid [2196F3](<../2196F3.md>) !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="cc:"]:before {
    color: [000746](<../000746.md>) !important;
    content: "📨 "
}```
            6. `Feedback Tags` 
                - [Feedback](<../Feedback.md>) 
#[[[Feedback](<../[[Feedback.md>): What's working]]
#[[[Feedback](<../[[Feedback.md>): What could be better]]
#[[[Feedback](<../[[Feedback.md>): [Suggestions](<../Suggestions.md>)]]
                    - ```css
:root {
  --color:[FFFFFF](<../FFFFFF.md>);
  --padding:2px 5px 2px 5px;
  --font-size: 13px;
  --line-height: 1em;
  --font-weight: 500;
  --border-radius: 5px 5px 5px 5px;
  --position:relative;
  
}

span.rm-page-ref[data-tag="Feedback"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: var(--padding);
    line-height: 1em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Feedback"]:before {
    content: '📣'
}

span.rm-page-ref[data-tag="[Feedback](<../Feedback.md>): What's working"] {
    background: [609a62](<../609a62.md>);
    color: [FFFFFF](<../FFFFFF.md>);
    padding: 3px 8px;
    line-height: 1em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="[Feedback](<../Feedback.md>): What's working"]:before {
    content: '📣😃'
}

span.rm-page-ref[data-tag="[Feedback](<../Feedback.md>): What could be better"] {
    background: [6775c3](<../6775c3.md>);
    color: [FFFFFF](<../FFFFFF.md>);
    padding: 3px 8px;
    line-height: 1em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="[Feedback](<../Feedback.md>): What could be better"]:before {
    content: '📣😕'
}

span.rm-page-ref[data-tag="[Feedback](<../Feedback.md>): [Suggestions](<../Suggestions.md>)"] {
    background: [0b8bc5](<../0b8bc5.md>);
    color: [FFFFFF](<../FFFFFF.md>);
    padding: 3px 8px;
    line-height: 1em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="[Feedback](<../Feedback.md>): [Suggestions](<../Suggestions.md>)"]:before {
    content: '📣💬'
}```
                - `#[Bug Reports-[[resolved](<../Bug Reports-[[resolved.md>)]]
                    - ```css
span.rm-page-ref[data-tag="Bug Reports"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Bug Reports"]:before {
    content: '🐛 '
}
```
                - `#[Roam Enhancement Requests](<../Roam Enhancement Requests.md>)
                    - ```css
span.rm-page-ref[data-tag="Roam Enhancement Requests"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Roam Enhancement Requests"]:before {
    content: '🚀 '
}```
            7. `Processing Tags` 
                - `[SRS](<../SRS.md>)
                    - ```css
span.rm-page-ref[data-tag="SRS"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="SRS"]:before {
    content: '🔁'
}```
                - `#[grab-attachment](<../grab-attachment.md>)
                    - ```css
span.rm-page-ref[data-tag="grab-attachment"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="grab-attachment"]:before {
    content: '📎'
}```
                - `#[connect-to](<../connect-to.md>)
                    - ```css
span.rm-page-ref[data-tag="connect-to"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="connect-to"]:before {
    content: '🔗'
}```
                - `#[find-connections](<../find-connections.md>)
                    - ```css
span.rm-page-ref[data-tag="find-connections"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="find-connections"]:before {
    content: '👀'
}```
                - `[find-reference](<../find-reference.md>)
                    - ```css
span.rm-page-ref[data-tag="find-reference"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="find-reference"]:before {
    content: '🔍'
}```
                - `#[how-should-I-tag-this](<../how-should-I-tag-this.md>)
                    - ```css
span.rm-page-ref[data-tag="how-should-I-tag-this"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="how-should-I-tag-this"]:before {
    content: '❔'
}```
            8. `Highlight Tags`
                - [Highlights](<../Highlights.md>)
                    - ```css
span.rm-page-ref[data-tag="Highlights"] {
    background: [FFC107](<../FFC107.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Highlights"]:before {
    content: ''
}```
                - `#[My Wins](<../My Wins.md>)
                    - ```css
span.rm-page-ref[data-tag="My Wins"] {
    background: [4CAF50](<../4CAF50.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="My Wins"]:before {
    content: '🏆'
}```
                - #[Key Concepts](<../Key Concepts.md>)
                    - ```css
span.rm-page-ref[data-tag="Key Concepts"] {
    background: [4CAF50](<../4CAF50.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Key Concepts"]:before {
    content: '🗝'
}```
                - [The BAGEL Method](<../The BAGEL Method.md>)
                    - #[Big Idea](<../Big Idea.md>)
                        - ```css
span.rm-page-ref[data-tag="Big Idea"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Big Idea"]:before {
    content: '🔵'
}```
                    - #[Antagonism](<../Antagonism.md>)
                        - ```css
span.rm-page-ref[data-tag="Antagonism"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Antagonism"]:before {
    content: '🔴'
}```
                    - #[General Noteworthy](<../General Noteworthy.md>)
                        - ```css
span.rm-page-ref[data-tag="General Noteworthy"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="General Noteworthy"]:before {
    content: '🟡'
}```
                    - #[External Reference](<../External Reference.md>)
                        - ```css
span.rm-page-ref[data-tag="External Reference"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="External Reference"]:before {
    content: '🟠'
}```
                    - #[List of Ideas](<../List of Ideas.md>)
                        - ```css
span.rm-page-ref[data-tag="List of Ideas"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="List of Ideas"]:before {
    content: '🟢'
}```
                - `#[Random Review](<../Random Review.md>)
                    - ```css
span.rm-page-ref[data-tag="Random Review"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Random Review"]:before {
    content: '🎲'
}```
            9. `Daily Tags`
                - `#[Writing & Reflection](<../Writing & Reflection.md>)
                    - ```css
span.rm-page-ref[data-tag="Writing & Reflection"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Writing & Reflection"]:before {
    content: '💬'
}```
                - `#[Today I Learned](<../Today I Learned.md>)
                    - ```css
span.rm-page-ref[data-tag="Today I Learned"] {
    background: [9C27B0](<../9C27B0.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Today I Learned"]:before {
    content: '⚡️'
}```
                - `#[Morning Journal](<../Morning Journal.md>)
                    - ```css
span.rm-page-ref[data-tag="Morning Journal"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Morning Journal"]:before {
    content: '🌞'
}```
                - `#[Evening Journal](<../Evening Journal.md>)
                    - ```css
span.rm-page-ref[data-tag="Evening Journal"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Evening Journal"]:before {
    content: '🌛'
}```
            10. `[Quote](<../Quote.md>) (inline block ref)
                - ```css
span.rm-page-ref[data-tag="Quote"] {
    background: [607D8B](<../607D8B.md>) !important;
    color: rgb(255,255,255) !important;
    padding: 1px 5px;
 	font-size: 13px;
    line-height: 1em;
    font-weight: 600;
  	border-radius: 4px 4px 4px 20px;
}


span.rm-page-ref[data-tag="Quote"]:before {
    content: '✦'
}
```
            11. `#[Actions Taken](<../Actions Taken.md>)
            12. `#[Action Items](<../Action Items.md>)
                - ```css
span.rm-page-ref[data-tag="Action Items"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Action Items"]:before {
    content: '🚩'
}```
            13. `#[Focus Mode](<../Focus Mode.md>)
            14. `#[The Zettelkasten](<../The Zettelkasten.md>)
                - ```css
span.rm-page-ref[data-tag="The Zettelkasten"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="The Zettelkasten"]:before {
    content: '⚡'
}```
            15. `#[Focus Mode (plus)](<../Focus Mode (plus).md>)
                - ```css
span.rm-page-ref[data-tag="Focus Mode (plus)"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Focus Mode (plus)"]:before {
    content: '🎯'
}```
            16. `#[Housekeeping](<../Housekeeping.md>)
                - ```css
span.rm-page-ref[data-tag="Housekeeping"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Housekeeping"]:before {
    content: '🧹'
}```
            17. `#[Quick Capture](<../Quick Capture.md>)
                - ```css
span.rm-page-ref[data-tag="Quick Capture"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Quick Capture"]:before {
    content: '📱'
}```
            18. `[Flag](<../Flag.md>)
                - ```css
span.rm-page-ref[data-tag="Flag"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag"]:before {
    content: '🚩'
}```
            19. `[Problems](<../Problems.md>)
                - ```css
span.rm-page-ref[data-tag="Problems"] {
    background: [C52D22](<../C52D22.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            20. `[Resolved](<../Resolved.md>)
                - ```css
span.rm-page-ref[data-tag="Resolved"] {
    color: [1ea20d](<../1ea20d.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            21. `[Happenings](<../Happenings.md>)
                - ```css
span.rm-page-ref[data-tag="Happenings"] {
    background: [0DCAAC](<../0DCAAC.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            22. `[Disabled](<../Disabled.md>)
                - ```css
span.rm-page-ref[data-tag="Disabled"] {
    background: [B82419](<../B82419.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            23. `[Important](<../Important.md>)
                - ```css
span.rm-page-ref[data-tag="Important"] {
    background: [0BE100](<../0BE100.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            24. `[Urgent](<../Urgent.md>)
                - ```css
span.rm-page-ref[data-tag="Urgent"] {
    background: [D90000](<../D90000.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            25. `Status/ tags`
                - ```css
span.rm-page-ref[data-tag="Status/Sent"] {
    background: [03A9F4](<../03A9F4.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Resolved"] {
    background: [8BC34A](<../8BC34A.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Closed"] {
    background: [000000](<../000000.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Completed"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Incomplete"] {
    color: [607D8B](<../607D8B.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Waiting-For"] {
    color: [795548](<../795548.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/On-Hold"] {
    color: [6A6A6A](<../6A6A6A.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Dropped"] {
    color: [C30D00](<../C30D00.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Active"] {
    color: [2196F3](<../2196F3.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Approved"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Someday|Maybe"] {
    color: [467C96](<../467C96.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Not-Completed, Carried"] {
    color: [FF9800](<../FF9800.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Enabled"] {
    background: [B1D7B1](<../B1D7B1.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            26. `Alert/ tags`
                - ```css
span.rm-page-ref[data-tag="Alert/Not Populated"] {
    color: [6F6F6F](<../6F6F6F.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            27. `Flag/ tags`
                - ```css
span.rm-page-ref[data-tag="Flag/Favourite"] {
    color: [FF3C7E](<../FF3C7E.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Highlight"] {
    color: [FFC107](<../FFC107.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Important"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Urgent"] {
    color: [D72D21](<../D72D21.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Deferred"] {
    color: [8C21D7](<../8C21D7.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Non-Important"] {
    color: [686868](<../686868.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Non-Urgent"] {
    color: [686868](<../686868.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Needs-Review"] {
    color: [FF9800](<../FF9800.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            28. `SCC/ tags`
                - ```css
span.rm-page-ref[data-tag="SCC/No Contact Yet"] {
    background: [C7291D](<../C7291D.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="SCC/In Progress"] {
    background: [FFC107](<../FFC107.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="SCC/Completed"] {
    background: [4CAF50](<../4CAF50.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="SCC/Transfer"] {
    background: [3F51B5](<../3F51B5.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}```
            29. Personas [Experiments](<../Experiments.md>)
                - Examples
                    - [P](<../P.md>):Self Your inner self talk
                    - [P](<../P.md>):Loving Love thyself
                    - [P](<../P.md>):Critic One's inner critical voice
                - ```css
/***************/
/** personas **/
/**************/

[data-tag="P:Self"]{
  background: [DFDDD5](<../DFDDD5.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 10px;
  color:brown;
}

[data-tag="P:Loving"]{
  background: [e2d0cb](<../e2d0cb.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 8px;
  color: red;
}

[data-tag="P:Critic"]{
  background: [C4CBB7](<../C4CBB7.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 10px;
  color:brown;
}

[data-tag="P:Self"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [DFDDD5](<../DFDDD5.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}

[data-tag="P:Loving"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [e2d0cb](<../e2d0cb.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}

[data-tag="P:Critic"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [C4CBB7](<../C4CBB7.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}```
            30. [Personas](https://www.rodrigofranco.com/roam-personas-css.html)
                - Examples
                    - #[P:Self](<../P:Self.md>) Inner Self Talk
                    - #[P:Loving](<../P:Loving.md>) Love thyself
                    - #[P:Critic](<../P:Critic.md>) Hard on yourself
                - ```css
/***************/
/** personas **/
/**************/

[data-tag="P:Self"]{
  background: [DFDDD5](<../DFDDD5.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 10px;
  color:black;
}

[data-tag="P:Loving"]{
  background: [e2d0cb](<../e2d0cb.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 8px;
  color:red;
}

[data-tag="P:Critic"]{
  background: [C4CBB7](<../C4CBB7.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 10px;
  color: brown;
}

[data-tag="P:Self"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [DFDDD5](<../DFDDD5.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}

[data-tag="P:Loving"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [e2d0cb](<../e2d0cb.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}

[data-tag="P:Critic"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [C4CBB7](<../C4CBB7.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}```
            31. **Archive**
                - `Evergreen tags` ([Legacy](<../Legacy.md>))
                    - ```css
span.rm-page-ref[data-tag="Groves"] {
    background: [009678](<../009678.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="Evergreens"] {
    background: [0DBAC6](<../0DBAC6.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}
```
                - ```html
/* Custom data tags */

span.rm-page-ref[data-tag="highlight"] {
    background: [FFC107](<../FFC107.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="key concept"] {
    background: [673AB7](<../673AB7.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="question"] {
    background: [673AB7](<../673AB7.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="questions"] {
    background: [673AB7](<../673AB7.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="ideas"] {
    background: [00BCD4](<../00BCD4.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SRS"] {
    background: [795548](<../795548.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="articles"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="meetings"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="flag"] {
    background: [FF9800](<../FF9800.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="conversations"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="lectures"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="examples"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="feedback"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="bug-reports"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="bug-reports"]:before {
    content: '🐛 '
}

span.rm-page-ref[data-tag="enhancement requests"] {
    background: [009688](<../009688.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="enhancement requests"]:before {
    content: '🚀 '
}

span.rm-page-ref[data-tag="Status/Sent"] {
    background: [03A9F4](<../03A9F4.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Status/Resolved"] {
    background: [8BC34A](<../8BC34A.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Status/Closed"] {
    background: [000000](<../000000.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="TwitterPost"] {
    background: [81D5ED](<../81D5ED.md>);
    color: white;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Literature Notes"] {
    background: [9769FF](<../9769FF.md>);
    color: white;
    padding: 3px 7px;
    font-weight: 500;
    line-height: 2em;
}


span.rm-page-ref[data-tag="Groves"] {
    background: [009678](<../009678.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Evergreens"] {
    background: [0DBAC6](<../0DBAC6.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Seedlings"] {
    color: [0dbac6](<../0dbac6.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Alert/Not Populated"] {
    color: [6F6F6F](<../6F6F6F.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Favourite"] {
    color: [FF3C7E](<../FF3C7E.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Highlight"] {
    color: [FFC107](<../FFC107.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Important"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Urgent"] {
    color: [D72D21](<../D72D21.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Deferred"] {
    color: [8C21D7](<../8C21D7.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Non-Important"] {
    color: [686868](<../686868.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Non-Urgent"] {
    color: [686868](<../686868.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Completed"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Waiting-For"] {
    color: [795548](<../795548.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/On-Hold"] {
    color: [6A6A6A](<../6A6A6A.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Dropped"] {
    color: [C30D00](<../C30D00.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Active"] {
    color: [2196F3](<../2196F3.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Approved"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Someday|Maybe"] {
    color: [467C96](<../467C96.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Not-Completed, Carried"] {
    color: [FF9800](<../FF9800.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Needs-Review"] {
    color: [FF9800](<../FF9800.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}


span.rm-page-ref[data-tag="projects"] {
    color: [0D58C6](<../0D58C6.md>);
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"] {
    color: [FCB815](<../FCB815.md>);
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"]:before {
    content: '✦ '
}

span.rm-page-ref[data-tag="Illustrated Notes"] {
    color: [7172FC](<../7172FC.md>);
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Garden Notes"] {
    color: [9DBC13](<../9DBC13.md>);
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Video Tutorial"] {
    color: [db3b8d](<../db3b8d.md>);
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Essay"] {
    background: [ADCB2A](<../ADCB2A.md>);
    color: [fff](<../fff.md>);
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Livestream"] {
    color: [B979CF](<../B979CF.md>);
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Talk"] {
    background: [7172FC](<../7172FC.md>);
    color: [fff](<../fff.md>);
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="waiting"] {
    background: [9C27B0](<../9C27B0.md>);
    color: [fff](<../fff.md>);
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Researching"] {
    background: [FF9D66](<../FF9D66.md>);
    color: [fff](<../fff.md>);
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Synthesising"] {
    background: [FC766F](<../FC766F.md>);
    color: [fff](<../fff.md>);
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Alive"] {
    background: [EE5F85](<../EE5F85.md>);
    color: [fff](<../fff.md>);
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Mindsweep"] {
    background: [999999](<../999999.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="InternetExploration"] {
    background: [999999](<../999999.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="INBOX"] {
    background: [999999](<../999999.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="transcript"] {
    background: [999999](<../999999.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="NOTES"] {
    background: [999999](<../999999.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Under Construction"] {
    background: [8a8a8a](<../8a8a8a.md>);
    color: [fff](<../fff.md>);
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="In the News"] {
    color: [737272](<../737272.md>);
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="problems"] {
    background: [C52D22](<../C52D22.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}     

span.rm-page-ref[data-tag="Resolved"] {
    color: [1ea20d](<../1ea20d.md>);
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
} 

span.rm-page-ref[data-tag="Daily Big 3"] {
    background: [238AFF](<../238AFF.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Morning Journal"] {
    background: [FFC107](<../FFC107.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Evening Journal"] {
    background: [7723FF](<../7723FF.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Happenings"] {
    background: [0DCAAC](<../0DCAAC.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Weekly Preview"] {
    background: [20AA4C](<../20AA4C.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="important"] {
    background: [0BE100](<../0BE100.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="urgent"] {
    background: [D90000](<../D90000.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Status/Enabled"] {
    background: [13CC11](<../13CC11.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Disabled"] {
    background: [B82419](<../B82419.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}



span.rm-page-ref[data-tag="*Roaming Notes*"] {
    background: [FF9800](<../FF9800.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SCC/No Contact Yet"] {
    background: [C7291D](<../C7291D.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SCC/In Progress"] {
    background: [FFC107](<../FFC107.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SCC/Completed"] {
    background: [4CAF50](<../4CAF50.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SCC/Transfer"] {
    background: [3F51B5](<../3F51B5.md>);
    color: [fff](<../fff.md>);
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}```
        2. Functional CSS
            - Fix sidebar editing height issue [Status](<../Status.md>)/Enabled
                - ```css
/* When editing page title in sidebar this prevents it from having weird height issues */
[right-sidebar](<../right-sidebar.md>) .rm-title-textarea {
    width: 95%;
}```
            - Buttons & Word Count [Status](<../Status.md>)/Enabled
                - ```css
/* Buttons in Block Text */
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: [D1D1D1](<../D1D1D1.md>);
  font-size: 12px;
/*  line-height: 12px;*/
  padding: 2px 4px 2px 4px; 
  min-height: 0px;
}

/* Buttons in Block References */
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: [D1D1D1](<../D1D1D1.md>);
  font-size: 12px;
/*  line-height: 12px;*/
  padding: 2px 4px 2px 4px; 
  min-height: 0px;
}

/* Buttons in Zoom Masks */
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: [D1D1D1](<../D1D1D1.md>);
  font-size: 12px;
/*  line-height: 12px;*/
  padding: 2px 4px 2px 4px; 
  min-height: 0px;
}```
            - Scope Highlighting ((This colors the vertical lines to show your mouse location and the bullet that you are editing))
                - ```ruby

.roam-block-container  div.roam-block-container {
box-shadow: -2px 0px [BFCCD6](<../BFCCD6.md>));
transition: box-shadow 1s;
}

.roam-block-container div.roam-block-container:hover {
box-shadow: -2px 0px [FF877E](<../FF877E.md>);
transition:  box-shadow 0.5s;
}

.roam-block-container:focus-within > .rm-block-main > div:nth-child(1) 
.rm-bullet .rm-bullet__inner  
{
background-color: [FF877E](<../FF877E.md>);
}```
        3. Core User Interface ([e.g.](<../e.g..md>), Headings)
            - Headings
                - Preview
                    - # Heading 1
                        - ## Heading 2
                            - ### Heading 3
                - Settings
                    - ```css
:root {
  --fnt-page-title: 		/*-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif*/;
  --fnt-h1:       			/*-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif*/;
  --fnt-h2:       			/*-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif*/;
  --fnt-h3:       			/*-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif*/;
  --fnt-size-page-title: 	22px;
  --fnt-size-h1:       		14px;
  --fnt-size-h2:       		14px;
  --fnt-size-h3:       		14px;
  --fnt-style-h1:			normal;
  --fnt-style-h2:			normal;
  --fnt-style-h3:			normal;
  --fnt-weight-h1:			500;
  --fnt-weight-h2:			500;
  --fnt-weight-h3:			500;
}```
                - Headings
                    - ```css
h1.level2,
.rm-level2, 
.rm-heading-level-2 > .rm-block__self .rm-block__input {
  color: var(--fg-h2);
}

.rm-level1, 
.rm-heading-level-1 > .rm-block__self .rm-block__input {
  color: var(--fg-h1);
}

.rm-level3, 
.rm-heading-level-3 > .rm-block__self .rm-block__input {
  color: var(--fg-h3);
}

.roam-body .roam-app h1,
.rm-level1, 
.rm-heading-level-1 > .rm-block__self .rm-block__input {
/*  font-family: var(--fnt-h1);*/
  font-size: var(--fnt-size-h1);
  font-weight: var(--fnt-weight-h1);
  font-style: var(--fnt-style-h1);
}

h1.level2,
.rm-level2, 
.rm-heading-level-2 > .rm-block__self .rm-block__input {
/*  font-family: var(--fnt-h2)!important; */
  font-size: var(--fnt-size-h2);
  font-weight: var(--fnt-weight-h2);
  font-style: var(--fnt-style-h2);
}

.rm-level3, 
.rm-heading-level-3 > .rm-block__self .rm-block__input {
/*  font-family: var(--fnt-h3); */
  font-size: var(--fnt-size-h3);
  font-weight: var(--fnt-weight-h3);
  font-style: var(--fnt-style-h3);
}

.roam-body .roam-app h1,
.roam-body .roam-app .roam-main .roam-article .rm-title-display {
/*  font-family: var(--fnt-page-title)!important; */
  font-size: var(--fnt-size-page-title);
  color: var(--fg-h1);
}```
            - Block Reference styling [Status](<../Status.md>)/Enabled
                - ```css
.rm-block-ref > span:before {
  content: '| ';
  font-weight: 700;
  color: [FF9800](<../FF9800.md>)
}```
            - Page Reference Underlines & Nested Links [Status](<../Status.md>)/Enabled
                - Example
                    - [[[E:](<../[[E:.md>) active vs passive resurfacing]]
                - Code
                    - V3
                        - ```css
:root {
  --fg-reference-underline: [136BA2](<../136BA2.md>);
  --fg-reference-underline-hover: [136BA2](<../136BA2.md>);
}

/*Reference Links*/
.rm-page-ref--link{
    /*background: linear-gradient(0deg, var(--fg-reference-underline) 1px, white 1px, transparent 1px)*/;
    /*background-position: 0 100%*/;
  	/*border-bottom: var(--fg-reference-underline) 1px;*/
    padding-bottom: 0px;
  	/*line-height: 24px;*/
}
.rm-page-ref--link:hover{
    background: linear-gradient(0deg, var(--fg-reference-underline-hover) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    text-decoration: none;
    padding-bottom: 0px;
    /*line-height: 24px;*/
}

.rm-page-ref--link .rm-page-ref--link {
  	/*background: linear-gradient(0deg, var(--fg-reference-underline) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    padding-bottom: 3px;
    line-height: 28px;
}
.rm-page-ref--link .rm-page-ref--link:hover {
  	background: linear-gradient(0deg, var(--fg-reference-underline-hover) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    padding-bottom: 3px;
    /*line-height: 28px;*/
}

.rm-page-ref--link .rm-page-ref--link .rm-page-ref--link {
	/*background: linear-gradient(0deg, var(--fg-reference-underline) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    padding-bottom: 6px;
    /*line-height: 32px;*/
}
.rm-page-ref--link .rm-page-ref--link .rm-page-ref--link:hover {
	background: linear-gradient(0deg, var(--fg-reference-underline-hover) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    padding-bottom: 6px;
    /*line-height: 32px;*/
}

/*Namespaces*/
/*.rm-page-ref--namespace{
    background: linear-gradient(0deg, var(--fg-reference-underline) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    padding-bottom: 0px;
}
.rm-page-ref--namespace:hover{
    background: linear-gradient(0deg, var(--fg-reference-underline-hover) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    text-decoration: none;
    padding-bottom: 0px;
}```
            - External Links [Status](<../Status.md>)/Enabled
                - V2
                    - ```css
/*Aliases - internal & external*/
.rm-alias--external {
  color: var(--fg-link);
    text-decoration: none!important;
    border-bottom: 1px dashed;
}

.rm-alias--external:hover {
	color: var(--fg-link-hover);
    text-decoration: none!important;
    border-bottom: 1px dashed;
}

.rm-alias--external:after {
  content: ' ↗';```
            - Page Reference Brackets [Status](<../Status.md>)/Enabled
                - ```ruby
.rm-page-ref__brackets{
  display:none;
}```
        4. Other Styling
            - Heading Styling
                - ```c++
.rm-ref-page-view-title {
 	font-weight: 600;
	font-size: 1.5em;
 }```
                - ```clojure
.rm-level1 {
    padding-top: 10px
}

.rm-level2 {
    font-size: 1.5em;
  	font-weight: 600;
    padding-top: 8px
}
.rm-level3 {
    color: [000000](<../000000.md>);
    font-weight: 600;
    font-size: 1.3em;
    padding-top: 8px
}
.rm-page-ref {
    color: [0885ff](<../0885ff.md>);
}
.rm-page-ref-link-color {
    color: [0885ff](<../0885ff.md>);
    font-weight: 600;
}
.rm-ref-page-view-title {
 	font-weight: 600;
 }

[right-sidebar](<../right-sidebar.md>) h1.level2 a {
    color: [000000](<../000000.md>) !important;  
  	font-weight: 400;
    text-decoration: none;
}

/* the location tag is necessary for the above lines to distinguish from external links */```
            - Headings & font [Status](<../Status.md>)/Enabled
                - ```css
*h1  {
  	font-size: 2.5em;
}

[roam-right-sidebar-content](<../roam-right-sidebar-content.md>) h1.rm-title-display {
  	font-size: 1.8em
}

h2,
h3,
h4,
h5,
h6 {
    font-family: "Lato", sans-serif;
    font-size: 3em;
}

.rm-page-ref-link-color {
    color: [2179F3](<../2179F3.md>);
    font-weight: 400;
}
a {
    color: [2179F3](<../2179F3.md>);
}```
            - Left side-bar [Status](<../Status.md>)/Enabled
                - ```ruby
/* Left Sidebar reformatting */

.roam-body .roam-app .roam-sidebar-container {
    background-color: white;
    border-right: 1px [eee](<../eee.md>) solid;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page,
.roam-body .roam-app .roam-sidebar-container > * {
    opacity: 80%;
    box-shadow: none;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
    background: white;
    color: black;
    opacity: 100%;
}```
            - Alias Styling
                - ```clojure
.rm-alias.rm-alias-page {
  	color: [0884ff](<../0884ff.md>) ;
  	font-weight: 600;
}

.rm-alias.rm-alias-page:hover {
  	color: rgb(17,153,55) ;
  	font-weight: 600;
}

.rm-alias.rm-alias-external {
  	color: [0884ff](<../0884ff.md>);
}

.rm-alias.rm-alias-external:hover {
  	color: rgb(17,153,55) ;
  	font-weight: 600;
}```
            - Link Formatting (naked)
                - ```clojure
/* link formatting: */

a {
    color: rgb(17,153,55);  
  	font-weight: 400;
 	text-decoration: none;
}

a:hover {
    color: rgb(0,0,0);  
  	font-weight: 400;
  	text-decoration: none;
}```
            - Reference Page in sidebar
                - ```clojure
.rm-ref-page-view-title span {
  	color: [000000](<../000000.md>);
  	font-weight: 600;
  	text-decoration: none !important; 	
}

.rm-ref-page-view-title:hover span {
  	color: rgb(17,153,55);
  	text-decoration: none !important; 	
}```
            - Round Check-Boxes
                - ```php
.checkmark {
  border-radius: 50% !important;
}```
            - Query Display Options
                - ```css
/* RR change: MINIMIZE QUERIES: add any one of the following tags 
before the beginning of your query (in the same block):

    [min-title](<../min-title.md>) = hides the page reference link / page title
    [min-con](<../min-con.md>) = hides the contextual reference information (breadcrumbs)
    [minimal](<../minimal.md>) = hides both the title and the context
    [min-q](<../min-q.md>) = hides the query string, similar to legacy behavior
    [min-all](<../min-all.md>) = hides everything — title, context, and query string
	[page-focus](<../page-focus.md>) = only displays pages

inspired by Matt Goldenberg */

[data-tag="minimal"], 
[data-tag="minimal"] + .rm-query .rm-title-arrow-wrapper,
[data-tag="minimal"] + .rm-query .zoom-mentions-view {
  display:none!important; /* hide page reference (title) and mention context (breadcrumbs) */
}
[data-tag="min-title"], [data-tag="min-title"] + .rm-query .rm-title-arrow-wrapper {
display:none!important; /* hide page reference (title) */
}
[data-tag="min-con"], [data-tag="min-con"] + .rm-query .zoom-mentions-view {
  display:none !important;  /* hide mention context (breadcrumbs) */
}
[data-tag="min-q"], 
[data-tag="min-q"] + .rm-query .rm-query-title {
  display:none !important;  /* hide the query string */
}
[data-tag="min-all"], 
[data-tag="min-all"] + .rm-query .zoom-mentions-view,
[data-tag="min-all"] + .rm-query .rm-title-arrow-wrapper,
[data-tag="min-all"] + .rm-query .rm-query-title {
  display:none !important;  /* hide everything */
}
[data-tag="minimal"] + .rm-query .rm-query-title::after,
[data-tag="min-title"] + .rm-query .rm-query-title::after,
[data-tag="min-con"] + .rm-query .rm-query-title::after{
  content: " [minimal](<../minimal.md>)" /* add a tag to the query string to indicate this query has been minimized */
}

/* Personal addition */
[data-tag="page-focus"], 
[data-tag="page-focus"] + .rm-query .zoom-mentions-view,
[data-tag="page-focus"] + .rm-query .rm-reference-item,
[data-tag="page-focus"] + .rm-query .rm-caret,
[data-tag="page-focus"] + .rm-query .rm-query-title {
  display:none !important;  /* hide everything */
}```
            - Link Symbol [Status](<../Status.md>)/Enabled
                - ```css
.rm-alias-external:before {
    content: '🔗'
}```
                - 
    - Feature Expansions
        - Split Screen
        - Split Tags
            - ```javascript
/* Split Screen CSS for Roam                 */
/* "Assembled" and tweaked by @DavidCrandall */
/* https://davidcrandallwrites.com           */
/* https://davidcrandallwrites.com/split-screen-and-rtl-custom-css-scripts-for-roam/ */
/*                                           */
/* Added tags by @garybasin                  */


/* tags */

.rm-page-ref-tag {
    font-size: 0.8em;
    font-weight: bold;  
    padding: 6px;
    margin: 4px;
    border-radius: 5px;
    border: 1px [bdbdbd](<../bdbdbd.md>) dotted;
}

[data-tag="me"] {
    /* Styles */
    color: [000](<../000.md>);
    background-color: [c9e33e](<../c9e33e.md>);
}

[data-tag="ps"] {
    color: white;
    background-color: [5353ff](<../5353ff.md>);
}

[data-tag="kap"] {
    color: white;
    background-color: [ff5f5f](<../ff5f5f.md>);
}

[data-tag="Sini"] {
    color: white;
    background-color: [55993a](<../55993a.md>);
}

[data-tag="Roam-Highlights"] {
    color: [b7b7b7](<../b7b7b7.md>);
    background-color: [ffffb4](<../ffffb4.md>);
}

/****************************/

/* change main font */

body,
html,
div,
textarea {
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
}

/* change font for all headings */

h1,
h1 div,
h1 textarea,
.rm-level1 div,
[right-sidebar](<../right-sidebar.md>) .rm-level2, /* page headings in right sidebar */
.rm-reference-main .rm-level3 , /* page headings in referenced items */
.rm-level1 textarea,
.roam-log-preview h1,
h1.rm-title-display,
h1.rm-title-display textarea, 
.level1,
.level2 {
  --font-family: "Fira Code", Menlo, monospace;
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  font-weight: 500 !important;
  --letter-spacing: -0.08em;
}

h2,
h2 div,
h2 textarea,
h3,
h3 div,
h3 textarea {
  --font-family: "Fira Code", Menlo, monospace;
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  color: [333](<../333.md>) !important;
}

/*a {
    color: [106ba3](<../106ba3.md>); 
}*/

/* less space below page heading */

.roam-body .roam-app .roam-main .roam-article .rm-title-display {
  margin-bottom: 10px;
}


h1.level2 {
    font-size: 36px !important;
}

/* Main block - remove centering */

.roam-center {
  --align-item: left;
  flex-basis: 40% !important;
}



/* lighter bullets */

[right-sidebar](<../right-sidebar.md>) .controls .roam-bullet-closed,
.controls .roam-bullet-closed {
  background: none;
  border: 1px solid silver;
}

.simple-bullet-inner {
  opacity: 0.3;
}

/* lighter vertical guides */

/* Hard to see with the light ones... -Gary
.block-border-left {
  border-color: [eee](<../eee.md>);
}*/


.roam-block-container h1 {
  font-weight: 300;
  font-size: 26px;
  color: black;
}

.roam-block-container h2 {
  font-weight: 600;
  font-size: 18px;
  color: black;
}

/* align checkboxes better */

label.check-container {
  margin-bottom: 11px;
  margin-right: 3px;
}

/* align checkboxes in zoomed-in headings */

.rm-level1 label.check-container {
  margin-bottom: 17px;
  margin-right: -3px;
}

/* don't shrink block references */

.rm-block-ref {
  font-size: 1em;
  padding: 0;
  margin: 0;
  border-bottom: 0.5px solid [91a8d2](<../91a8d2.md>); /* darker -Gary */
}

.rm-block-ref label.check-container {
  margin-bottom: 12px;
}

/* wider blocks -Gary */
.rm-block-text {
    max-width: 700px;
}


/* don't need "SHORTCUTS" heading */

.starred-pages-wrapper .flex-h-box {
  display: none;
}

.starred-pages-wrapper > div:first-child {
  margin: 0 -18px;
}

/* more subtle logo */

[roam-sidebar-logo](<../roam-sidebar-logo.md>) img {
  opacity: 0.4;
}
[roam-sidebar-logo](<../roam-sidebar-logo.md>) span {
  display: none;
}

/* fade loading astrolabe */

.loading-astrolabe img {
  opacity: 0.2;
}

/* lighter sidebar background */

[right-sidebar](<../right-sidebar.md>) {
  background-color: rgba(216, 225, 232, 0.2) !important; 
  /* rgba(216, 225, 232, 0.3) */
  border-left: 1px solid [ddd](<../ddd.md>) !important;
}

/* sidebar sections */

[roam-right-sidebar-content](<../roam-right-sidebar-content.md>) > div {
  border-bottom: 1px solid [ddd](<../ddd.md>) !important;
  margin: 0 !important;
  padding: 10px 4px 10px 50px;
}

/* sidebar section headings */

[roam-right-sidebar-content](<../roam-right-sidebar-content.md>) > div > div:first-child {
  margin-left: -10px;
}

/* rule under top section of left sidebar */

.roam-sidebar-content > div:first-child {
  padding: 4px 16px !important;
  margin-bottom: 8px;
  border-bottom: 1px solid rgb(57, 75, 89);
}

/* rule under topbar */

.roam-topbar {
  border-bottom: 1px solid [eee](<../eee.md>);
}

/* crumbs */

.rm-reference-item
  > div:first-child
  > div:first-child
  div
  span:not(.bp3-icon-chevron-right),
.roam-article
  > div:first-child:not(.roam-log-container)
  > div:first-child
  div
  span:not(.bp3-icon-chevron-right) {
  font-size: 12px;
  line-height: 1.3;
  color: [bbb](<../bbb.md>) !important;
  /* truncate to smaller width, use css for ellipsis */
  --max-width: 1000px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  padding: 2px !important;
}

.rm-reference-item
  > div:first-child
  > div:first-child
  div
  span:hover:not(.bp3-icon-chevron-right),
.roam-article
  > div:first-child:not(.roam-log-container)
  > div:first-child
  div
  span:hover:not(.bp3-icon-chevron-right) {
  color: black !important;
}

/* chevrons in crumbs */

.roam-reference-item > div > div:first-child .bp3-icon-chevron-right,
.roam-article
  > div
  > div:first-child:not(.roam-log-container)
  .bp3-icon-chevron-right {
  font-size: 1em;
  margin: 0 3px;
  color: [ddd](<../ddd.md>) !important;
}

/* no checkboxes in crumbs */

.roam-reference-item
  > div:first-child:not(.roam-log-container)
  > div:first-child
  label.check-container,
.roam-article
  > div:first-child:not(.roam-log-container)
  > div:first-child
  label.check-container {
  display: none;
}

/* link buttons for referenced items */

.rm-reference-main button {
  border: 1px solid [eee](<../eee.md>);
  border-radius: 0.3em;
  font-size: 0.8em;
}

.rm-reference-main button:hover {
  border-color: [ccc](<../ccc.md>);
}

/* referenced item section headings */

.rm-reference-main {
  --border-top: 1px solid [ededed](<../ededed.md>);
}

.flex-h-box {
    padding-top: 0px !important;
}

.rm-reference-main .flex-h-box {
  min-height: 30px;
}

.rm-reference-main strong {
  color: [222](<../222.md>);
  font-size: 0.9em;
  --background-color: rgba(216, 225, 232, 0.3);
}

/* remove background from referenced items */

.rm-reference-item {
  padding: 6px 0 0 0;
  margin: 6px 0 0 0;
  border-top: 1px solid [eee](<../eee.md>);
  background: none;
}

/* slightly bigger page headings under referenced items */
.rm-reference-main .rm-level3 {
  font-size: 1.6em;
}

/* search */

.rm-find-or-create-wrapper {
  flex: 0 1 100% !important;
}

.rm-find-or-create-wrapper .bp3-input {
  border: none !important;
  box-shadow: none !important;
}

/* highlights */

.roam-highlight {
  --background-color: [c2f9fa](<../c2f9fa.md>);
}

/* links */

a.rm-alias.rm-alias-external {
    color: [b33ba9](<../b33ba9.md>) !important;
}

a {
    color: [b33ba9](<../b33ba9.md>);  
}

.rm-page-ref-link-color {
    color: [106ba3](<../106ba3.md>);
}

.rm-ref-page-view-title a{
    color: [106ba3](<../106ba3.md>);
    font-weight: bold;
}


.level2 a{
    color: [106ba3](<../106ba3.md>);
}

/* tweets -- doesn't work */

.twitter-tweet {
    font-size: 7px;
}

/* embeds */

/*.rm-embed-container {
    border: 1px;
    border-color: black;
    border-style: solid;
}*/```
        - Make Wide
            - ```javascript
.roam-center div:first-child {
            padding-right: calc((100% - 900px) / 2) !important;
        }
        .roam-block-container {
            max-width: calc(1024px - 80px);
        }
        .roam-center .roam-article .rm-block-text {
            max-width: 580px;
        }
        [right-sidebar](<../right-sidebar.md>) {
            [roam-right-sidebar-content](<../roam-right-sidebar-content.md>) {
                .rm-block-text {
                    max-width: 680px;
                }
            }
        }
```
        - Fix for orange blocks
            - ```css
[find-or-create-input](<../find-or-create-input.md>) {
   outline: none!important;
}```
        - Width of sidebar
            - ```css
/*This does a decent job of expanding one pane or the other depending on how much space each needs. It'll give you a little more room.*/
.roam-center {
    flex-basis: auto !important;
    resize: horizontal !important;
    overflow: auto !important;
}```
    - User Interface Elements
    - **[Inbox](<../Inbox.md>):**
        - [ ] Add [Suggestions](<../Suggestions.md>) to [roam/css](<../roam/css.md>)

# Backlinks
## [Agenda](<Agenda.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [CSS](<CSS.md>)
- **[Redirect](<../Redirect.md>):** [roam/css](<../roam/css.md>)

## [Decisions](<Decisions.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [Development Requests](<Development Requests.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [Experiments](<Experiments.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [Frameworks](<Frameworks.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [January 25th, 2021](<January 25th, 2021.md>)
7. Added [roam/css](<../roam/css.md>)

5. [x] Add [Processes](<../Processes.md>) to [roam/css](<../roam/css.md>)

11. [ ] Improve [roam/css](<../roam/css.md>)

- [e.g.](<../e.g..md>) "[ ] Improve [roam/css](<../roam/css.md>)

1. Added [roam/css](<../roam/css.md>)

## [January 28th, 2021](<January 28th, 2021.md>)
- Hey [~[[leekeifon](<../~[[leekeifon.md>)]] 👋🏼! Nice to meet you via the graph. I saw your note [here](((FehE8jv6_))) and wanted to point you to [roam/css](<../roam/css.md>)

## [January 30th, 2021](<January 30th, 2021.md>)
- [ ] Reorganize the [roam/css](<../roam/css.md>)

- [minimal](<../minimal.md>) {{[query](<../query.md>): {and: [Evergreen](<../Evergreen.md>) {not: {or: [E:](<../E:.md>) [roam/css](<../roam/css.md>)}

## [January 31st, 2021](<January 31st, 2021.md>)
- "[Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

- [Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

10. "Yup " — "[Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

- "[Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

## [Members](<Members.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [People](<People.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [Thoughts](<Thoughts.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [roam/css](<roam/css.md>)
- [ ] Add [Suggestions](<../Suggestions.md>) to [roam/css](<../roam/css.md>)

