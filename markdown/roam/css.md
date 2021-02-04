- #Announcements
    - ## Please document any changes to the CSS under a `#[[Change Log]]` tag within your [[DNP Section]]
- Related:: [[roam/js]]
- Tips:: 
    - add `?disablejs=true&disablecss=true` to the end of your roam graph URL, to load without CSS or JS #Troubleshooting
- ### Shortcuts::
    - [Colors](((ClLqIfFSn)))
    - [Tag Styling](((yAzEsiUsx))) ((This needs to be tidied up significantly... ((r1E6gBj56))))
        - [Collections Tags](((JNVnlLDxv))) 
        - [Notifications & Mentions](((01X6uO5N8)))
    - [Headings](((nL58k_bhI)))
    - [Page References](((kJ_piMpzy)))
    - [Block References](((xcLgPdvs0)))
    - [External Links](((r3wJzzQJP)))
    - [Aliases](((MLfGQ-X-L)))
    - [Nested Links](((y9rumn-yn)))
    - [Queries](((KOuJf-Smr)))
- Contents::
    - ## Settings
        - Colors
            - Color Scheme
                - > Use names for consistent colors throughout your them
                - Base
                    - ```css
:root {
  --cl-white:			#ffffff;
  --cl-gray-50:			#f4f5f5;
  --cl-gray-100:		#e5e6e6;
  --cl-gray-200: 		#dcdcdc;
  --cl-gray-300: 		#bdbdbd;
  --cl-gray-400: 		#99999d;
  --cl-gray-500: 		#797a79;
  --cl-gray-600: 		#646464;
  --cl-gray-700: 		#454545;
  --cl-gray-800: 		#272727;
  --cl-gray-900:		#1a1a1a;
  --cl-black:			#000000;
  --cl-green-700: 		#1a8917;
  --cl-blue-50:			#e8f2ff;
  --cl-blue-200:		#BFDBFE;
  --cl-yellow-200:		#FDE68A;
  --cl-red-500: 		#fe3c30;
  --cl-orange-500:	 	#fe9500;
  --cl-yellow-500: 		#fecc00;
  --cl-green-500: 		#27cd41;
  --cl-blue-500: 		#007aff;
  --cl-indigo-500: 		#5756d5;
  --cl-purple-500: 		#af52de;
  --cl-pink-500: 		#fe2e55;	
  --cl-brown-500: 		#a2845e;
  --cl-beige-200:		#eec170;
  --cl-beige-500:		#c8963e;
  --cl-beige-700:		#472515;
}```
                - Togetic
                    - ```css
:root {
/*Togetic #176*/
  --cl-togetic-gray-500:  #737b83;
  --cl-togetic-gray-300:  #acc5bd;
  --cl-togetic-gray-100:  #d5eeee;
  --cl-togetic-red-500:   #bd1808;
  --cl-togetic-red-300:   #de4139;
  --cl-togetic-blue-500:  #1062bd;
  --cl-togetic-blue-300:  #2994e6;
}```
                - Wobbufet
                    - ```css
:root {
  /* CSS HEX */
  --uranian-blue: #a4deffff;
  --aero: #73bdf6ff;
  --blue-jeans: #52aceeff;
  --yale-blue: #20528bff;
  --gray-web: #838383ff;
  --davys-grey: #525252ff;
  --dark-orange: #ff8b00ff;
  --persimmon: #de5200ff;
  --rufous: #a41000ff;
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
                    - ```clojure
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
                        - This is [a link](http://link.com), this is a reference to a page [[Test Page]], this is a [[Project/Complete Job Search & Get Hired]] namespace, this is a double underline [[[[R:]] Remote Work (podcasts)]]
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
                        - #tag1 #tag2
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
                        - {{[[calc]]: 31 + 11}}
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
  --bg-code-fat-cursor:				#7e7;
  --bg-code-fat-cursor-mark:		rgba(20, 255, 20, 0.5);
  --bg-code-fat-cursor-animate:		#7e7;
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
  --bg-code-fat-cursor:				#7e7;
  --bg-code-fat-cursor-mark:		rgba(20, 255, 20, 0.5);
  --bg-code-fat-cursor-animate:		#7e7;
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
                        - {{[[diagram]]}}
                            - A
                            - B
                - Embed
                    - > Changes the background color of embed blocks
                    - Preview
                        - Sample Data
                            - Embed 1
                                - {{[[embed]]: ((ZuyIjM6mE))}}
                            - Embed 2
                                - {{[[embed]]: ((oVEJn3mnp))}}
                            - Embed 3
                        - {{[[embed]]: ((CR-dOUiRZ))}}
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
                        - {{[[kanban]]}}
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
                        - {{[[query]]: {and: [[TODO]] [[December 30th, 2020]]}}}
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
                        - {{[[table]]}}
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
                        - {{[[TODO]]}} This is a todo
                        - {{[[DONE]]}} This is a finished todo
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
                - 
                    - ```css
:root {
  --note-tag-color:				var(--cl-gray-700);
}

@media (prefers-color-scheme: dark) {
  :root {
  	--note-tag-color:			var(--cl-gray-200);
  }
}```
    - ## Elements
        1. Tag Styling 
            1. `GTD Tags`
                - `GTD Tags`
                    - `#INBOX
#Inbox
#Projects
#Goals
#[[Follow Up]]
#Mindsweep
#Waiting
#[[Waiting-[[resolved]]]]
#Tracking
#[[Daily Big 3]]
#[[Plan My Day]]
#[[Weekly Preview]]
#[[Next Steps]]
#GTD
                        - ```css
:root {
  --background:#607D8B;
  --color:#FFFFFF;
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

span.rm-page-ref[data-tag="Waiting-[[resolved]]"] {
    background: #607D8B;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Waiting-[[resolved]]"]:before {
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
                - `#[[Reference Notes]]
                    - ```css
span.rm-page-ref[data-tag="Reference Notes"] {
	background-image: linear-gradient(90deg, #BEDFF8, #BEDFF8, #BEDFF8);
	background-size: 100%;
    color: #000000;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - `#[[Seedlings]]
                    - ```css
span.rm-page-ref[data-tag="Seedlings"] {
    color: #FFFFFF !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FFEFBA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #A6DA69, #A6DA69);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #A6DA69, #A6DA69); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}




```
                - `#Annotations
                    - ```css
span.rm-page-ref[data-tag="Annotations"] {
    background: #795548E2;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - `#[[Fleeting Notes]]
                    - ```css
span.rm-page-ref[data-tag="Fleeting Notes"] {
    color: #1A1718 !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FFEFBA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FFEFBA, #FFEFBA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #FFEFBA, #FFEFBA); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}




```
                - `#[[Literature Notes]] [[Test]]
                    - ```css
span.rm-page-ref[data-tag="Literature Notes"] {
	background-image: linear-gradient(90deg, #3A98E3, #3A98E3, #3A98E3);
	background-size: 100%;
    color: #FFFFFF;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}



```
                - `#[[Evergreen Notes]] [[Test]]
                    - ```css
span.rm-page-ref[data-tag="Evergreen Notes"] {
	background-image: linear-gradient(90deg, #507B58, #507B58, #507B58);
	background-size: 100%;
    color: #EEF2EE;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

/* span.rm-page-ref[data-tag="Permanent Notes"] + span[data-link-title] {
     background: #DCE5DE8C !important;
     color: #F3F7F2 !important;
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
    border-left-color: #507B58;
    border-width: 10px;
    margin-top: -10px;
}

span.rm-page-ref[data-tag="Permanent Notes"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #507B58;
    border-width: 10px;
    margin-top: -10px;
}



```
                - `#[[Zettel Questions]]
                    ```clojure
span.rm-page-ref[data-tag="Zettel Questions"] {
    color: #FFFFFF !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #BC6DCA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #BC6DCA, #BC6DCA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #BC6DCA, #BC6DCA); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}




```
                - `#[[Branching Notes]] [[Test]]
                    - ```css
span.rm-page-ref[data-tag="Branching Notes"] {
background: #B79891;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #94716B, #94716B);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #94716B, #94716B); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

	background-size: 100%;
    color: #EEF2EE;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

/* span.rm-page-ref[data-tag="Branching Notes"] + span[data-link-title] {
     background: #B7989128 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 5px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0px 5px 5px 0px;
     margin-left: -5px;
} */





```
                - `#[[Intermediary Notes]]
                    - ```css
span.rm-page-ref[data-tag="Intermediary Notes"] {
	color: #1A1718 !important;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #607D8B68;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #607D8B68, #607D8B68);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #607D8B68, #607D8B68); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

  
}

```
                - `#[[Project Ideas]]
                    - ```css
span.rm-page-ref[data-tag="Project Ideas"] {
	color: #1A1718 !important;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FF572268;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FF572268, #FF572268);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #FF572268, #FF572268); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

  
}

```
                - #Evergreen
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
                        - Example: "#Evergreen Prefer note titles with complete phrases to sharpen claims"
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
                - #[[Community Note]]
                    - Tag
                        - ```css
span.rm-page-ref[data-tag="Community Note"]:before {
    content: '⛺ '
}

span.rm-page-ref[data-tag="Community Note"]:after {
    content: ':'
}

span.rm-page-ref[data-tag="Community Note"] {
 color: var(--note-tag-color) !important;
 padding: 1px 1px !important;
 font-weight: 700 !important;
}```
                    - In Block Reference
                        - Example: "#Evergreen Prefer note titles with complete phrases to sharpen claims"
                        - ```css
.rm-block-ref > span > span.rm-page-ref--tag[data-tag="Evergreen"]{
  /*display: none;*/
  font-size: .1px;
  line-height: 1.5em;
}

.rm-block-ref > span > span.rm-page-ref--tag[data-tag="Community Note"]:before{
  font-size: 12px;
  margin-right: -5px;
}```
            3. `Areas Tags`
                - `#[[Administration]]
            4. `Data-type Tags`
                - `#Articles
                    - ```css
span.rm-page-ref[data-tag="Articles"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Books
                    - ```css
span.rm-page-ref[data-tag="Books"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Experiments
                    - ```css
span.rm-page-ref[data-tag="Experiments"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Tweets
                    - ```css
span.rm-page-ref[data-tag="Tweets"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Conversations and Meetings]]
                    - ```css
span.rm-page-ref[data-tag="Conversations and Meetings"] {
    background: #607D8B;
    color: #fff;
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
                - `#Podcasts
                    - ```css
span.rm-page-ref[data-tag="Podcasts"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Meetings
                    - ```css
span.rm-page-ref[data-tag="Meetings"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Conversations
                    - ```css
span.rm-page-ref[data-tag="Conversations"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Discoveries
                    - ```css
span.rm-page-ref[data-tag="Discoveries"] {
    background: #03A9F4;
    color: #fff;
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
                - `#Lectures
                    - ```css
span.rm-page-ref[data-tag="Lectures"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Learning Objectives]]
                    - ```css
span.rm-page-ref[data-tag="Learning Objectives"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Recommendations
                    - ```css
span.rm-page-ref[data-tag="Recommendations"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[I]]
                    - ```css
span.rm-page-ref[data-tag="I"] {
    background: #607D8B;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="I"]:before {
    content: '💡'
}```
                - `#Ideas
                    - ```css
span.rm-page-ref[data-tag="Ideas"] {
    background: #607D8B;
    color: #fff;
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
                - `#Jokes
                    - ```css
span.rm-page-ref[data-tag="Jokes"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Frameworks
                    - ```css
span.rm-page-ref[data-tag="Frameworks"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Goal Ideas]]
                    - ```css
span.rm-page-ref[data-tag="Goal Ideas"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Graph Mentorship]]
                    - ```css
span.rm-page-ref[data-tag="Graph Mentorship"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Prompt Ideas]]
                    - ```css
span.rm-page-ref[data-tag="Prompt Ideas"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Quotes
                    - ```css
span.rm-page-ref[data-tag="Quotes"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Prompts
                    - ```css
span.rm-page-ref[data-tag="Prompts"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#People
                    - ```css
span.rm-page-ref[data-tag="People"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Members
                    - ```css
span.rm-page-ref[data-tag="Members"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Observations
                    - ```css
span.rm-page-ref[data-tag="Observations"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Opportunities
                    - ```css
span.rm-page-ref[data-tag="Opportunities"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Examples
                    - ```css
span.rm-page-ref[data-tag="Examples"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Transcript
                    - ```css
span.rm-page-ref[data-tag="Transcript"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#missing-list
                    - ```css
span.rm-page-ref[data-tag="missing-list"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Conventions
                    - ```css
span.rm-page-ref[data-tag="Conventions"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Processes
                    - ```css
span.rm-page-ref[data-tag="Processes"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Resources
                    - ```css
span.rm-page-ref[data-tag="Resources"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Stories
                    - ```css
span.rm-page-ref[data-tag="Stories"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Sprints
                    - ```css
span.rm-page-ref[data-tag="Sprints"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Predictions
                    - ```css
span.rm-page-ref[data-tag="Predictions"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Replies
                    - ```css
span.rm-page-ref[data-tag="Replies"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Idioms
                    - ```css
span.rm-page-ref[data-tag="Idioms"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Timestamps
                    - ```css
span.rm-page-ref[data-tag="Timestamps"] {
    background: #9E9E9E;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - `#Tips
                    - ```css
span.rm-page-ref[data-tag="Tips"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Tensions
                    - ```css
span.rm-page-ref[data-tag="Tensions"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#Templates
                    - ```css
span.rm-page-ref[data-tag="Templates"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Q]]
                    - ```clojure
span.rm-page-ref[data-tag="Context Questions"] {
    background: #607D8B;
    color: #fff;
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
                - `#[[Open Questions]]
                    - ```clojure
span.rm-page-ref[data-tag="Open Questions"] {
    background: #607D8B;
    color: #fff;
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
                - `#Q
                    - ```css
span.rm-page-ref[data-tag="Q"] {
    background: #607D8B;
    color: #fff;
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
                - `#Shownotes
                    - ```css
span.rm-page-ref[data-tag="Shownotes"] {
    background: #9E9E9E;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - `#[[Weather Report]]
                    - ```css
span.rm-page-ref[data-tag="Weather Report"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Tips & Tricks]]
                    - ```css
span.rm-page-ref[data-tag="Tips & Tricks"] {
    background: #4CAF50;
    color: #fff;
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
                - `#Questions
                    - ```css
span.rm-page-ref[data-tag="Questions"] {
    background: #607D8B;
    color: #fff;
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
                - #Reply-from [[Your Name]]
                    - ```css
span.rm-page-ref[data-tag="Reply-from"] {
	background-image: linear-gradient(to right, #CD4CE3AD,#CD4CE3AD);
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
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
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
    border-left-color: #CD4CE3AD;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Reply-from"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #CD4CE3AD;
    border-width: 11px;
    margin-top: -11px;
}


```
                - `#Conversation
                    - ```css
span.rm-page-ref[data-tag="Conversation"] {
    background: #9C27B0;
    color: #fff;
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
                - `#Announcements
                    - ```css
span.rm-page-ref[data-tag="Announcements"] {
    background: #F44336;
    color: #fff;
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
                - `#[[Change Log]]
                    - ```css
span.rm-page-ref[data-tag="Change Log"] {
    background: #4CAF50;
    color: #fff;
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
                - `#Promptstorming
                    - ```css
span.rm-page-ref[data-tag="Promptstorming"] {
    background: #98160C;
    color: #fff;
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
                - `#[[Help Wanted]]
                    - ```css
span.rm-page-ref[data-tag="Help Wanted"] {
    background: #9C27B0;
    color: #fff;
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
                - `#[[Dice Roll]]
                    - ```css
span.rm-page-ref[data-tag="Dice Roll"] {
    background: #009688;
    color: #fff;
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
                - `#[[Scratchpad]]
                    - ```css
span.rm-page-ref[data-tag="Scratchpad"] {
    background: #607D8B;
    color: #fff;
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
                - `#[[Bookmarks]]
                    - ```css
span.rm-page-ref[data-tag="Bookmarks"] {
    background: #2196F3;
    color: #fff;
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
                - `#[[The Main Feed]]
                    - ```css
span.rm-page-ref[data-tag="The Main Feed"] {
    background: #607D8B;
    color: #fff;
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
                - `#[[Daily Log]]
                    - ```css
span.rm-page-ref[data-tag="Daily Log"] {
    background: #FF9800;
    color: #fff;
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
                - `#[[Daily Activities]]
                    - ```css
span.rm-page-ref[data-tag="Daily Activities"] {
    background: #4CAF50;
    color: #fff;
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
                - #[[My Daily Notes]] [[Your Name]]
                    - ```css
span.rm-page-ref[data-tag="My Daily Notes"] {
	background-image: linear-gradient(to right, #607D8B,#607D8B);
	background-size: 100%;
    color: rgb(255,255,255);
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="My Daily Notes"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
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
    border-left-color: #607D8B;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="My Daily Notes"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #607D8B;
    border-width: 11px;
    margin-top: -11px;
}```
                - #[[Posted by]] [[Your Name]]
                - `#[[Chat]]
                    - ```css
span.rm-page-ref[data-tag="Chat"] {
    background: #2196F3;
    color: #fff;
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
                - `#Chat [[Your Name]] #@ [[Beau Haan 📌]]`
                    - ```ruby
span.rm-page-ref[data-tag="Chat"] {
	background-image: linear-gradient(to right, #4c8dc9,#4c8dc9);
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
 
}

/* span.rm-page-ref[data-tag="Chat"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
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
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Chat"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}
*/
```
                - #Reply
                    - ```css
span.rm-page-ref[data-tag="Reply"] {
	background: #CD4CE3AD;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}
  
/* span.rm-page-ref[data-tag="Reply"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
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
    border-left-color: #CD4CE3AD;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Reply"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #CD4CE3AD;
    border-width: 11px;
    margin-top: -11px;
}
*/
```
                - #Question [[Their Name]]
                - #Help [[Your Name]]
                    - ```css
span.rm-page-ref[data-tag="Help"] {
	background-image: linear-gradient(to right, #FF9800,#FF9800);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Help"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
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
    border-left-color: #FF9800;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Help"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #FF9800;
    border-width: 11px;
    margin-top: -11px;
}



```
                - #@ [[Their Name]]
                    - ```css
span.rm-page-ref[data-tag="@"] {
	background-image: linear-gradient(to right, #4c8dc9,#4c8dc9);
	background-size: 100%;
    color: #EEF2EE;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="@"] + span[data-link-title] {
     background: #e4ffe3 !important;
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
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="@"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}




```
                - #Polls
                    - ```css
span.rm-page-ref[data-tag="Polls"] {
    color: white !important;
    padding: 3px 5px 3px 5px;
	font-size: 13px;
    line-height: 1em;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FFEFBA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FFFFFF, #FFEFBA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #5856d6, #5856d6); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}






```
                - #Video
                    - ```css
span.rm-page-ref[data-tag="Video"] {
	background-image: linear-gradient(to right, #0D71EB,#0D71EB);
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
     border: 1px solid #0D71EB;
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
    border-left-color: #0D71EB;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Video"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #0D71EB;
    border-width: 11px;
    margin-top: -11px;
}




```
                - Notifications & Mentions:
                    - Example::
                        - [[@[[Their Name]]]]
                        - [[cc:[[Their Name]]]]
                        - [[~[[Your Name]]]]
                        - [[^[[Your Name]]]]
                    - ```css
span[data-link-title^="@"] {
        border: 2px solid #a76800 !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="@"]:before {
    color: #000746 !important;
    content: "🚨unread "
}

span[data-link-title^="~"] {
        border: 2px solid #02B920 !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="~"]:before {
    color: #000746 !important;
    content: "✅read "
}

span[data-link-title^="^"] {
        border: 2px solid #4CAF50 !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="^"]:before {
    color: #000746 !important;
    content: "💾saved "
}

span[data-link-title^="cc:"] {
        border: 2px solid #2196F3 !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="cc:"]:before {
    color: #000746 !important;
    content: "📨 "
}```
            6. `Feedback Tags` 
                - #Feedback 
#[[[[Feedback]]: What's working]]
#[[[[Feedback]]: What could be better]]
#[[[[Feedback]]: [[Suggestions]]]]
                    - ```css
:root {
  --color:#FFFFFF;
  --padding:2px 5px 2px 5px;
  --font-size: 13px;
  --line-height: 1em;
  --font-weight: 500;
  --border-radius: 5px 5px 5px 5px;
  --position:relative;
  
}

span.rm-page-ref[data-tag="Feedback"] {
    background: #009688;
    color: #fff;
    padding: var(--padding);
    line-height: 1em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Feedback"]:before {
    content: '📣'
}

span.rm-page-ref[data-tag="[[Feedback]]: What's working"] {
    background: #609a62;
    color: #FFFFFF;
    padding: 3px 8px;
    line-height: 1em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="[[Feedback]]: What's working"]:before {
    content: '📣😃'
}

span.rm-page-ref[data-tag="[[Feedback]]: What could be better"] {
    background: #6775c3;
    color: #FFFFFF;
    padding: 3px 8px;
    line-height: 1em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="[[Feedback]]: What could be better"]:before {
    content: '📣😕'
}

span.rm-page-ref[data-tag="[[Feedback]]: [[Suggestions]]"] {
    background: #0b8bc5;
    color: #FFFFFF;
    padding: 3px 8px;
    line-height: 1em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="[[Feedback]]: [[Suggestions]]"]:before {
    content: '📣💬'
}```
                - `#[[Bug Reports-[[resolved]]]]
                    - ```css
span.rm-page-ref[data-tag="Bug Reports"] {
    background: #009688;
    color: #fff;
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
                - `#[[Roam Enhancement Requests]]
                    - ```css
span.rm-page-ref[data-tag="Roam Enhancement Requests"] {
    background: #009688;
    color: #fff;
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
                - `#SRS
                    - ```css
span.rm-page-ref[data-tag="SRS"] {
    background: #009688;
    color: #fff;
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
                - `#[[grab-attachment]]
                    - ```css
span.rm-page-ref[data-tag="grab-attachment"] {
    background: #009688;
    color: #fff;
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
                - `#[[connect-to]]
                    - ```css
span.rm-page-ref[data-tag="connect-to"] {
    background: #009688;
    color: #fff;
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
                - `#[[find-connections]]
                    - ```css
span.rm-page-ref[data-tag="find-connections"] {
    background: #009688;
    color: #fff;
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
                - `#find-reference
                    - ```css
span.rm-page-ref[data-tag="find-reference"] {
    background: #009688;
    color: #fff;
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
                - `#[[how-should-I-tag-this]]
                    - ```css
span.rm-page-ref[data-tag="how-should-I-tag-this"] {
    background: #009688;
    color: #fff;
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
                - #Highlights
                    - ```css
span.rm-page-ref[data-tag="Highlights"] {
    background: #FFC107;
    color: #fff;
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
                - `#[[My Wins]]
                    - ```css
span.rm-page-ref[data-tag="My Wins"] {
    background: #4CAF50;
    color: #fff;
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
                - #[[Key Concepts]]
                    - ```css
span.rm-page-ref[data-tag="Key Concepts"] {
    background: #4CAF50;
    color: #fff;
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
                - [[The BAGEL Method]]
                    - #[[Big Idea]]
                        - ```css
span.rm-page-ref[data-tag="Big Idea"] {
    background: #9E9E9E;
    color: #fff;
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
                    - #[[Antagonism]]
                        - ```css
span.rm-page-ref[data-tag="Antagonism"] {
    background: #9E9E9E;
    color: #fff;
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
                    - #[[General Noteworthy]]
                        - ```css
span.rm-page-ref[data-tag="General Noteworthy"] {
    background: #9E9E9E;
    color: #fff;
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
                    - #[[External Reference]]
                        - ```css
span.rm-page-ref[data-tag="External Reference"] {
    background: #9E9E9E;
    color: #fff;
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
                    - #[[List of Ideas]]
                        - ```css
span.rm-page-ref[data-tag="List of Ideas"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Random Review]]
                    - ```css
span.rm-page-ref[data-tag="Random Review"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Writing & Reflection]]
                    - ```css
span.rm-page-ref[data-tag="Writing & Reflection"] {
    background: #607D8B;
    color: #fff;
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
                - `#[[Today I Learned]]
                    - ```css
span.rm-page-ref[data-tag="Today I Learned"] {
    background: #9C27B0;
    color: #fff;
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
                - `#[[Morning Journal]]
                    - ```css
span.rm-page-ref[data-tag="Morning Journal"] {
    background: #9E9E9E;
    color: #fff;
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
                - `#[[Evening Journal]]
                    - ```css
span.rm-page-ref[data-tag="Evening Journal"] {
    background: #9E9E9E;
    color: #fff;
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
            10. `#Quote (inline block ref)
                - ```css
span.rm-page-ref[data-tag="Quote"] {
    background: #607D8B !important;
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
            11. `#[[Actions Taken]]
            12. `#[[Action Items]]
                - ```css
span.rm-page-ref[data-tag="Action Items"] {
    background: #9E9E9E;
    color: #fff;
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
            13. `#[[Focus Mode]]
            14. `#[[The Zettelkasten]]
                - ```css
span.rm-page-ref[data-tag="The Zettelkasten"] {
    background: #607D8B;
    color: #fff;
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
            15. `#[[Focus Mode (plus)]]
                - ```css
span.rm-page-ref[data-tag="Focus Mode (plus)"] {
    background: #607D8B;
    color: #fff;
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
            16. `#[[Housekeeping]]
                - ```css
span.rm-page-ref[data-tag="Housekeeping"] {
    background: #9E9E9E;
    color: #fff;
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
            17. `#[[Quick Capture]]
                - ```css
span.rm-page-ref[data-tag="Quick Capture"] {
    background: #9E9E9E;
    color: #fff;
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
            18. `#Flag
                - ```css
span.rm-page-ref[data-tag="Flag"] {
    background: #9E9E9E;
    color: #fff;
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
            19. `#Problems
                - ```css
span.rm-page-ref[data-tag="Problems"] {
    background: #C52D22;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            20. `#Resolved
                - ```css
span.rm-page-ref[data-tag="Resolved"] {
    color: #1ea20d;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            21. `#Happenings
                - ```css
span.rm-page-ref[data-tag="Happenings"] {
    background: #0DCAAC;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            22. `#Disabled
                - ```css
span.rm-page-ref[data-tag="Disabled"] {
    background: #B82419;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            23. `#Important
                - ```css
span.rm-page-ref[data-tag="Important"] {
    background: #0BE100;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            24. `#Urgent
                - ```css
span.rm-page-ref[data-tag="Urgent"] {
    background: #D90000;
    color: #fff;
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
    background: #03A9F4;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Resolved"] {
    background: #8BC34A;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Closed"] {
    background: #000000;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Completed"] {
    color: #4CAF50;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Incomplete"] {
    color: #607D8B;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Waiting-For"] {
    color: #795548;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/On-Hold"] {
    color: #6A6A6A;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Dropped"] {
    color: #C30D00;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Active"] {
    color: #2196F3;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Approved"] {
    color: #4CAF50;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Someday|Maybe"] {
    color: #467C96;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Not-Completed, Carried"] {
    color: #FF9800;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Enabled"] {
    background: #4CAF50;
    color: #fff;
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
    color: #6F6F6F;
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
    color: #FF3C7E;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Highlight"] {
    color: #FFC107;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Important"] {
    color: #4CAF50;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Urgent"] {
    color: #D72D21;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Deferred"] {
    color: #8C21D7;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Non-Important"] {
    color: #686868;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Non-Urgent"] {
    color: #686868;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Flag/Needs-Review"] {
    color: #FF9800;
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
    background: #C7291D;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="SCC/In Progress"] {
    background: #FFC107;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="SCC/Completed"] {
    background: #4CAF50;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="SCC/Transfer"] {
    background: #3F51B5;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}```
            29. Personas #Experiments
                - Examples
                    - #P:Self Your inner self talk
                    - #P:Loving Love thyself
                    - #P:Critic One's inner critical voice
                - ```css
/***************/
/** personas **/
/**************/

[data-tag="P:Self"]{
  background: #DFDDD5;
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 10px;
  color:brown;
}

[data-tag="P:Loving"]{
  background: #e2d0cb;
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 8px;
  color: red;
}

[data-tag="P:Critic"]{
  background: #C4CBB7;
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
	border-left-color: #DFDDD5;
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
	border-left-color: #e2d0cb;
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
	border-left-color: #C4CBB7;
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}```
            30. [Personas](https://www.rodrigofranco.com/roam-personas-css.html)
                - Examples
                    - #[[P:Self]] Inner Self Talk
                    - #[[P:Loving]] Love thyself
                    - #[[P:Critic]] Hard on yourself
                - ```css
/***************/
/** personas **/
/**************/

[data-tag="P:Self"]{
  background: #DFDDD5;
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 10px;
  color:black;
}

[data-tag="P:Loving"]{
  background: #e2d0cb;
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 8px;
  color:red;
}

[data-tag="P:Critic"]{
  background: #C4CBB7;
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
	border-left-color: #DFDDD5;
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
	border-left-color: #e2d0cb;
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
	border-left-color: #C4CBB7;
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}```
            31. **Archive**
                - `Evergreen tags` (#Legacy)
                    - ```css
span.rm-page-ref[data-tag="Groves"] {
    background: #009678;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="Evergreens"] {
    background: #0DBAC6;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}
```
                - ```html
/* Custom data tags */

span.rm-page-ref[data-tag="highlight"] {
    background: #FFC107;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="key concept"] {
    background: #673AB7;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="question"] {
    background: #673AB7;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="questions"] {
    background: #673AB7;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="ideas"] {
    background: #00BCD4;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SRS"] {
    background: #795548;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="articles"] {
    background: #9E9E9E;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="meetings"] {
    background: #9E9E9E;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="flag"] {
    background: #FF9800;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="conversations"] {
    background: #9E9E9E;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="lectures"] {
    background: #9E9E9E;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="examples"] {
    background: #9E9E9E;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="feedback"] {
    background: #009688;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="bug-reports"] {
    background: #009688;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="bug-reports"]:before {
    content: '🐛 '
}

span.rm-page-ref[data-tag="enhancement requests"] {
    background: #009688;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="enhancement requests"]:before {
    content: '🚀 '
}

span.rm-page-ref[data-tag="Status/Sent"] {
    background: #03A9F4;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Status/Resolved"] {
    background: #8BC34A;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Status/Closed"] {
    background: #000000;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="TwitterPost"] {
    background: #81D5ED;
    color: white;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Literature Notes"] {
    background: #9769FF;
    color: white;
    padding: 3px 7px;
    font-weight: 500;
    line-height: 2em;
}


span.rm-page-ref[data-tag="Groves"] {
    background: #009678;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Evergreens"] {
    background: #0DBAC6;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Seedlings"] {
    color: #0dbac6;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Alert/Not Populated"] {
    color: #6F6F6F;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Favourite"] {
    color: #FF3C7E;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Highlight"] {
    color: #FFC107;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Important"] {
    color: #4CAF50;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Urgent"] {
    color: #D72D21;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Deferred"] {
    color: #8C21D7;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Non-Important"] {
    color: #686868;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Non-Urgent"] {
    color: #686868;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Completed"] {
    color: #4CAF50;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Waiting-For"] {
    color: #795548;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/On-Hold"] {
    color: #6A6A6A;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Dropped"] {
    color: #C30D00;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Active"] {
    color: #2196F3;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Approved"] {
    color: #4CAF50;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Someday|Maybe"] {
    color: #467C96;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Status/Not-Completed, Carried"] {
    color: #FF9800;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Flag/Needs-Review"] {
    color: #FF9800;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}


span.rm-page-ref[data-tag="projects"] {
    color: #0D58C6;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"] {
    color: #FCB815;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"]:before {
    content: '✦ '
}

span.rm-page-ref[data-tag="Illustrated Notes"] {
    color: #7172FC;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Garden Notes"] {
    color: #9DBC13;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Video Tutorial"] {
    color: #db3b8d;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Essay"] {
    background: #ADCB2A;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Livestream"] {
    color: #B979CF;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Talk"] {
    background: #7172FC;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="waiting"] {
    background: #9C27B0;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Researching"] {
    background: #FF9D66;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Synthesising"] {
    background: #FC766F;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Alive"] {
    background: #EE5F85;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Mindsweep"] {
    background: #999999;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="InternetExploration"] {
    background: #999999;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="INBOX"] {
    background: #999999;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="transcript"] {
    background: #999999;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="NOTES"] {
    background: #999999;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Under Construction"] {
    background: #8a8a8a;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="In the News"] {
    color: #737272;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="problems"] {
    background: #C52D22;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}     

span.rm-page-ref[data-tag="Resolved"] {
    color: #1ea20d;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
} 

span.rm-page-ref[data-tag="Daily Big 3"] {
    background: #238AFF;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Morning Journal"] {
    background: #FFC107;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Evening Journal"] {
    background: #7723FF;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Happenings"] {
    background: #0DCAAC;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Weekly Preview"] {
    background: #20AA4C;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="important"] {
    background: #0BE100;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="urgent"] {
    background: #D90000;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Status/Enabled"] {
    background: #13CC11;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Disabled"] {
    background: #B82419;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}



span.rm-page-ref[data-tag="*Roaming Notes*"] {
    background: #FF9800;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SCC/No Contact Yet"] {
    background: #C7291D;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SCC/In Progress"] {
    background: #FFC107;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SCC/Completed"] {
    background: #4CAF50;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="SCC/Transfer"] {
    background: #3F51B5;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}```
        2. Buttons & Word Count #Status/Enabled
            - ```css
/* Buttons in Block Text */
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: #D1D1D1;
  font-size: 12px;
/*  line-height: 12px;*/
  padding: 2px 4px 2px 4px; 
  min-height: 0px;
}

/* Buttons in Block References */
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: #D1D1D1;
  font-size: 12px;
/*  line-height: 12px;*/
  padding: 2px 4px 2px 4px; 
  min-height: 0px;
}

/* Buttons in Zoom Masks */
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: #D1D1D1;
  font-size: 12px;
/*  line-height: 12px;*/
  padding: 2px 4px 2px 4px; 
  min-height: 0px;
}```
        3. Scope Highlighting ((This colors the vertical lines to show your mouse location and the bullet that you are editing)) #Status/Enabled
            - ```css

.roam-block-container  div.roam-block-container {
box-shadow: -2px 0px #BFCCD6);
transition: box-shadow 1s;
}

.roam-block-container div.roam-block-container:hover {
box-shadow: -0.5px 0px #666666;
transition:  box-shadow 0.5s;
}

.roam-block-container:focus-within > .rm-block-main > div:nth-child(1) 
.rm-bullet .rm-bullet__inner  
{
background-color: #000000;
}```
        4. Query Display Options
            - V1
                - ```css
/* RR change: MINIMIZE QUERIES: add any one of the following tags 
before the beginning of your query (in the same block):

    #min-title = hides the page reference link / page title
    #min-con = hides the contextual reference information (breadcrumbs)
    #minimal = hides both the title and the context
    #min-q = hides the query string, similar to legacy behavior
    #min-all = hides everything — title, context, and query string
	#page-focus = only displays pages

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
  content: " #minimal" /* add a tag to the query string to indicate this query has been minimized */
}

/* Personal addition */
[data-tag="page-focus"], 
[data-tag="page-focus"] + .rm-query .zoom-mentions-view,
[data-tag="page-focus"] + .rm-query .rm-reference-item,
[data-tag="page-focus"] + .rm-query .rm-caret,
[data-tag="page-focus"] + .rm-query .rm-query-title {
  display:none !important;  /* hide everything */
}```
        5. Headings #Status/Enabled
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
        6. Page References #Status/Enabled
            - ```css
.rm-page-ref-link-color {
    color: #2179F3;
    font-weight: 400;
}
a {
    color: #2179F3;
}```
        7. Page Reference Brackets
            - ```ruby
.rm-page-ref__brackets{
  display:none;
}```
        8. Block Reference styling #Status/Enabled
            - ```css
.rm-block-ref > span:before {
  content: '| ';
  font-weight: 700;
  color: #FF9800
}```
        9. Page Reference Underlines & Nested Links #Status/Enabled
            - Example
                - [[[[E:]] active vs passive resurfacing]]
            - Code
                - V3
                    - ```css
:root {
  --fg-reference-underline: #136BA2;
  --fg-reference-underline-hover: #136BA2;
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
    padding-bottom: 2px;
    line-height: 28px;
}
.rm-page-ref--link .rm-page-ref--link:hover {
  	background: linear-gradient(0deg, var(--fg-reference-underline-hover) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    padding-bottom: 2px;
    /*line-height: 28px;*/
}

.rm-page-ref--link .rm-page-ref--link .rm-page-ref--link {
	/*background: linear-gradient(0deg, var(--fg-reference-underline) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    padding-bottom: 4px;
    /*line-height: 32px;*/
}
.rm-page-ref--link .rm-page-ref--link .rm-page-ref--link:hover {
	background: linear-gradient(0deg, var(--fg-reference-underline-hover) 1px, white 1px, transparent 1px);
    /*background-position: 0 100%;*/
    padding-bottom: 4px;
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
        10. External Links #Status/Enabled
            - V1
                - ```css
.rm-alias--external {
  color: var(--fg-link);
}

a[href^='http']:active, a[href^='http']:hover, a[href^='http']:focus {
    text-decoration: none!important;
    border-bottom: 1px dashed;
    color: #2196F3;;
}
a[href^='http']{
  color: #2196F3;
  text-decoration: none!important;
  border-bottom: 1px solid;
}```
        11. Alias Styling 
            - ```clojure
.rm-alias.rm-alias-page {
  	color: #0884ff ;
  	font-weight: 600;
}

.rm-alias.rm-alias-page:hover {
  	color: rgb(17,153,55) ;
  	font-weight: 600;
}

.rm-alias.rm-alias-external {
  	color: #0884ff;
}

.rm-alias.rm-alias-external:hover {
  	color: rgb(17,153,55) ;
  	font-weight: 600;
}```
        12. Prevent right sidebar title from jumping around when editing #Status/Enabled
            - ```css

#right-sidebar .rm-title-textarea {
    width: 95%;
}```
    - ### Patch Fixes
        - Fix for orange blocks ((Unsure purpose - BT))
            - ```css
#find-or-create-input {
   outline: none!important;
}```
    - ### Archive
        - Left side-bar 
            - ```ruby
/* Left Sidebar reformatting */

.roam-body .roam-app .roam-sidebar-container {
    background-color: white;
    border-right: 1px #eee solid;
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
        - Headings & font
            - ```clojure
*h1  {
  	font-size: 2.5em;
}

#roam-right-sidebar-content h1.rm-title-display {
  	font-size: 1.8em
}

h2,
h3,
h4,
h5,
h6 {
    font-family: "Lato", sans-serif;
    font-size: 3em;
}```
