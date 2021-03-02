- **[Conventions](<../Conventions.md>):**
    1. Nest code under examples
        - [Meta](<../Meta.md>)
            - ```css
```
    2. Add note under a #[Change Log](<../Change Log.md>) header in your Daily Notes Section, referencing the code block and detailing the change
    3. Try to use the standard set of colors & variables as much as possible!
- **[### Shortcuts](<../### Shortcuts.md>):**
    - [Colors](((ClLqIfFSn)))
    - [Tag Styling](((6w_N1hr1k)))
        - [Collections Tags](((JNVnlLDxv))) 
        - [Notifications & Mentions](Notifications & Mentions)
    - [Headings](((nL58k_bhI)))
    - [Page References](((kJ_piMpzy)))
    - [Block References](((xcLgPdvs0)))
    - [External Links](((r3wJzzQJP)))
    - [Aliases](((MLfGQ-X-L)))
    - [Nested Links](((y9rumn-yn)))
    - [Queries](((KOuJf-Smr)))
- **Settings & Variables:**
    - Colors
        - Color Scheme
            - > Use names for consistent colors throughout your them — `--cl-name-strength`
            - Colors
                - Black, White, Gray
                    - ```css
:root {
  --cl-white:    [ffffff](<../ffffff.md>);
  --cl-gray-100: [f8f9faff](<../f8f9faff.md>); /*--cultured*/
  --cl-gray-200: [e9ecefff](<../e9ecefff.md>); /*--cultured-2*/
  --cl-gray-300: [dee2e6ff](<../dee2e6ff.md>); /*--gainsboro*/
  --cl-gray-400: [ced4daff](<../ced4daff.md>); /*--light-gray*/
  --cl-gray-500: [adb5bdff](<../adb5bdff.md>); /*--cadet-blue-crayola*/
  --cl-gray-600: [6c757dff](<../6c757dff.md>); /*--slate-gray*/
  --cl-gray-700: [495057ff](<../495057ff.md>); /*--davys-grey*/
  --cl-gray-800: [343a40ff](<../343a40ff.md>); /*--gunmetal*/
  --cl-gray-900: [212529ff](<../212529ff.md>); /*--charleston-green*/
  --cl-black:    [000000](<../000000.md>);
}```
                - Red
                    - ```css
:root {
  --cl-red-100: [ffc2c4ff](<../ffc2c4ff.md>); /*--spanish-pink*/
  --cl-red-200: [f9acafff](<../f9acafff.md>); /*--light-pink*/
  --cl-red-300: [f3969aff](<../f3969aff.md>); /*--salmon-pink*/
  --cl-red-400: [ed8084ff](<../ed8084ff.md>); /*--light-coral*/
  --cl-red-500: [e86b6fff](<../e86b6fff.md>); /*--candy-pink*/
  --cl-red-600: [e2555aff](<../e2555aff.md>); /*--indian-red*/
  --cl-red-700: [dc3f45ff](<../dc3f45ff.md>); /*--rose-madder*/
  --cl-red-800: [d6292fff](<../d6292fff.md>); /*--amaranth-red*/
  --cl-red-900: [d0131aff](<../d0131aff.md>); /*--lava*/
}```
                - Orange
                    - ```css
:root {
  --cl-orange-100: [ffcdadff](<../ffcdadff.md>); /*--apricot:*/
  --cl-orange-200: [fbbe97ff](<../fbbe97ff.md>); /*--peach-crayola:*/
  --cl-orange-300: [f7af82ff](<../f7af82ff.md>); /*--macaroni-and-cheese:*/
  --cl-orange-400: [f3a06cff](<../f3a06cff.md>); /*--atomic-tangerine:*/
  --cl-orange-500: [f09257ff](<../f09257ff.md>); /*--atomic-tangerine-2:*/
  --cl-orange-600: [ec8341ff](<../ec8341ff.md>); /*--princeton-orange:*/
  --cl-orange-700: [e8742bff](<../e8742bff.md>); /*--spanish-orange:*/
  --cl-orange-800: [e46516ff](<../e46516ff.md>); /*--spanish-orange-2:*/
  --cl-orange-900: [e05600ff](<../e05600ff.md>); /*--persimmon:*/
}```
                - Yellow
                    - ```css
:root {
  --cl-yellow-100: [FDEAB4ff](<../FDEAB4ff.md>); /*--jasmine:*/
  --cl-yellow-200: [fbdc86ff](<../fbdc86ff.md>); /*--jasmine-2:*/
  --cl-yellow-300: [f7d473ff](<../f7d473ff.md>); /*--orange-yellow-crayola:*/
  --cl-yellow-400: [f3cc60ff](<../f3cc60ff.md>); /*--maize-crayola:*/
  --cl-yellow-500: [f0c54dff](<../f0c54dff.md>); /*--maize-crayola-2:*/
  --cl-yellow-600: [ecbd39ff](<../ecbd39ff.md>); /*--saffron:*/
  --cl-yellow-700: [e8b526ff](<../e8b526ff.md>); /*--orange-yellow:*/
  --cl-yellow-800: [e4ad13ff](<../e4ad13ff.md>); /*--goldenrod:*/
  --cl-yellow-900: [e0a500ff](<../e0a500ff.md>); /*--goldenrod-2:*/

}```
                - Green Yellow
                    - ```css
:root {
  --cl-green-yel-100: [eaecacff](<../eaecacff.md>);/*--pale-spring-bud:*/
  --cl-green-yel-200: [e1e39bff](<../e1e39bff.md>);/*--green-yellow-crayola:*/
  --cl-green-yel-300: [d8da8bff](<../d8da8bff.md>);/*--khaki-x-11-light-khaki:*/
  --cl-green-yel-400: [cfd17aff](<../cfd17aff.md>);/*--straw:*/
  --cl-green-yel-500: [c6c96aff](<../c6c96aff.md>);/*--dark-khaki:*/
  --cl-green-yel-600: [bcc059ff](<../bcc059ff.md>);/*--olive-green:*/
  --cl-green-yel-700: [b3b748ff](<../b3b748ff.md>);/*--olive-green-2:*/
  --cl-green-yel-800: [aaae38ff](<../aaae38ff.md>);/*--citron:*/
  --cl-green-yel-900: [a1a527ff](<../a1a527ff.md>);/*--citron-2:*/
}```
                - Green
                    - ```css
:root {
  --cl-green-100: [cae4a0ff](<../cae4a0ff.md>); /*--yellow-green-crayola:*/
  --cl-green-200: [bed991ff](<../bed991ff.md>); /*--yellow-green-crayola-2:*/
  --cl-green-300: [b2cf82ff](<../b2cf82ff.md>); /*--pistachio:*/
  --cl-green-400: [a5c473ff](<../a5c473ff.md>); /*--olivine:*/
  --cl-green-500: [99ba64ff](<../99ba64ff.md>); /*--olivine-2:*/
  --cl-green-600: [8daf55ff](<../8daf55ff.md>); /*--olivine-3:*/
  --cl-green-700: [81a446ff](<../81a446ff.md>); /*--moss-green:*/
  --cl-green-800: [749a37ff](<../749a37ff.md>); /*--olive-drab-3:*/
  --cl-green-900: [688f28ff](<../688f28ff.md>); /*--olive-drab-3-2:*/
}```
                - Green-Blue
                    - ```css
:root {
  --cl-green-blu-100: [a8dcd9ff](<../a8dcd9ff.md>);/*--powder-blue:*/ 
  --cl-green-blu-200: [9ad3d0ff](<../9ad3d0ff.md>);/*--middle-blue-green:*/ 
  --cl-green-blu-300: [8dc9c6ff](<../8dc9c6ff.md>);/*--middle-blue-green-2:*/ 
  --cl-green-blu-400: [7fc0bdff](<../7fc0bdff.md>);/*--green-sheen:*/ 
  --cl-green-blu-500: [72b7b3ff](<../72b7b3ff.md>);/*--green-sheen-2:*/ 
  --cl-green-blu-600: [64adaaff](<../64adaaff.md>);/*--verdigris:*/ 
  --cl-green-blu-700: [56a4a0ff](<../56a4a0ff.md>);/*--cadet-blue:*/ 
  --cl-green-blu-800: [499a97ff](<../499a97ff.md>);/*--cadet-blue-2:*/ 
  --cl-green-blu-900: [3b918dff](<../3b918dff.md>);/*--viridian-green:*/ 
}```
                - Blue (lighter shade)
                    - ```css
:root {
  --cl-blue-lt-100: [aec7efff](<../aec7efff.md>); /*--baby-blue-eyes:*/
  --cl-blue-lt-200: [a0bce9ff](<../a0bce9ff.md>); /*--baby-blue-eyes-2:*/
  --cl-blue-lt-300: [8fafe2ff](<../8fafe2ff.md>); /*--french-sky-blue:*/
  --cl-blue-lt-400: [7ea5e0ff](<../7ea5e0ff.md>); /*--little-boy-blue:*/
  --cl-blue-lt-500: [7099daff](<../7099daff.md>); /*--cornflower-blue:*/
  --cl-blue-lt-600: [5f8cd3ff](<../5f8cd3ff.md>); /*--united-nations-blue:*/
  --cl-blue-lt-700: [4c7eceff](<../4c7eceff.md>); /*--glaucous:*/
  --cl-blue-lt-800: [3770cbff](<../3770cbff.md>); /*--celtic-blue:*/
  --cl-blue-lt-900: [2b66c4ff](<../2b66c4ff.md>); /*--true-blue:*/}```
                - Blue
                    - ```css
:root {
  --cl-blue-100:   [dceff9ff](<../dceff9ff.md>); /*--alice-blue:*/
  --cl-blue-200:   [a7d9f1ff](<../a7d9f1ff.md>); /*--uranian-blue:*/
  --cl-blue-300:   [85c6e9ff](<../85c6e9ff.md>); /*--light-cornflower-blue:*/
  --cl-blue-400:   [5aaddcff](<../5aaddcff.md>); /*--blue-jeans:*/
  --cl-blue-500:   [389bd5ff](<../389bd5ff.md>); /*--carolina-blue:*/
  --cl-blue-600:   [1e7ac0ff](<../1e7ac0ff.md>); /*--star-command-blue:*/
  --cl-blue-700:   [0254a0ff](<../0254a0ff.md>); /*--usafa-blue:*/
  --cl-blue-800:   [014889ff](<../014889ff.md>); /*--yale-blue:*/
  --cl-blue-900:   [023a72ff](<../023a72ff.md>); /*--indigo-dye:*/
}```
                - Blue (Darker Shade)
                    - ```css
:root {
  --cl-blue-dk-100: [7a8fd8ff](<../7a8fd8ff.md>); /* --cornflower-blue:  */
  --cl-blue-dk-200: [6e85d0ff](<../6e85d0ff.md>); /* --glaucous:  */
  --cl-blue-dk-300: [6076c9ff](<../6076c9ff.md>); /* --han-blue:  */
  --cl-blue-dk-400: [526cc1ff](<../526cc1ff.md>); /* --han-blue-2:  */
  --cl-blue-dk-500: [455eb9ff](<../455eb9ff.md>); /* --liberty:  */
  --cl-blue-dk-600: [3f56aaff](<../3f56aaff.md>); /* --cerulean-blue:  */
  --cl-blue-dk-700: [3a4f99ff](<../3a4f99ff.md>); /* --y-in-mn-blue:  */
  --cl-blue-dk-800: [30448fff](<../30448fff.md>); /* --dark-cornflower-blue:  */
  --cl-blue-dk-900: [263a83ff](<../263a83ff.md>); /* --dark-cornflower-blue-2:  */}```
                - Violet
                    - ```css
:root {
  --cl-violet-100: [afb1d4ff](<../afb1d4ff.md>); /*--wild-blue-yonder*/
  --cl-violet-200: [a2a4caff](<../a2a4caff.md>); /*--blue-bell*/
  --cl-violet-300: [9597c0ff](<../9597c0ff.md>); /*--blue-bell-2*/
  --cl-violet-400: [888ab6ff](<../888ab6ff.md>); /*--cool-grey*/
  --cl-violet-500: [7b7eadff](<../7b7eadff.md>); /*--rhythm*/
  --cl-violet-600: [6e71a3ff](<../6e71a3ff.md>); /*--dark-blue-gray*/
  --cl-violet-700: [616499ff](<../616499ff.md>); /*--dark-blue-gray-2*/
  --cl-violet-800: [54578fff](<../54578fff.md>); /*--purple-navy*/
  --cl-violet-900: [474a85ff](<../474a85ff.md>); /*--purple-navy-2*/
}```
                - Purple
                    - ```css
:root {
  --cl-purple-100: [bfaed5ff](<../bfaed5ff.md>); /*--lilac*/
  --cl-purple-200: [b3a1cbff](<../b3a1cbff.md>); /*--glossy-grape*/
  --cl-purple-300: [a894c2ff](<../a894c2ff.md>); /*--glossy-grape-2*/
  --cl-purple-400: [9c87b8ff](<../9c87b8ff.md>); /*--purple-mountain-majesty*/
  --cl-purple-500: [907aaeff](<../907aaeff.md>); /*--purple-mountain-majesty-2*/
  --cl-purple-600: [846ca4ff](<../846ca4ff.md>); /*--middle-blue-purple*/
  --cl-purple-700: [795f9bff](<../795f9bff.md>); /*--royal-purple*/
  --cl-purple-800: [6d5291ff](<../6d5291ff.md>); /*--royal-purple-2*/
  --cl-purple-900: [614587ff](<../614587ff.md>); /*--cyber-grape*/
}```
            - Additional Color Schemes
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
        - Color Settings [Status](<../Status.md>)/Inactive
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
                        - This is [a link](http://link.com), this is a reference to a page [Test Page](<../Test Page.md>), this is a [Project/Complete Job Search & Get Hired](<../Project/Complete Job Search & Get Hired.md>) namespace, this is a double underline [Podcasts/Remote Work (podcasts)](<../Podcasts/Remote Work (podcasts).md>)
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
    - Fonts
        - Code Blocks
            - Code
                - ```css
:root {
  --fnt-size-inline-code:		12px;
  --fnt-size-code-block:		14px;
}

.CodeMirror .CodeMirror-code pre {
  font-size: var(--fnt-size-code-block);
  font-style: normal!important;
}

code {
  font-size: var(--fnt-size-inline-code);
  font-style: normal!important;
}

```
                - Example: `this is a code block`
- ### **Code:**
    - Elements
        - Tags
            - Variables
                - ```css
:root {
  /*
  Format:
  --tag-bg-cl-<family-name>: 	var(--cl-<color-name>);
  */
  --tag-bg-cl-gtd:		var(--cl-blue-500);
}```
            - Top-Section Tags
                - #[Community Notes](<../Community Notes.md>) [Roam Collective](<../Roam Collective.md>)
                    - ```css
span.rm-page-ref[data-tag="Community Notes"] {
	background-image: linear-gradient(to right, var(--cl-gray-800),var(--cl-gray-800));
	background-size: 100%;
    color: var(--cl-white);
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Community Notes"] + span[data-link-title] {
     background: var(--cl-gray-400) !important;
     color: var(--cl-gray-800) !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Community Notes"]:after, span.rm-page-ref[data-tag="Post"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Community Notes"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: var(--cl-gray-800);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Community Notes"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: var(--cl-gray-800);
    border-width: 11px;
    margin-top: -11px;
}```
                - [Announcements](<../Announcements.md>)
                    - ```css
span.rm-page-ref[data-tag="Announcements"] {
    background: var(--cl-red-600);
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Announcements"]:before {
    content: '📢';
}```
                - #[Daily Activities](<../Daily Activities.md>)
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
                - #[The Main Feed](<../The Main Feed.md>)
                    - ```css
span.rm-page-ref[data-tag="The Main Feed"] {
	background: var(--cl-orange-600);
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
                - #[Chat](<../Chat.md>)
                    - ```css
span.rm-page-ref[data-tag="Chat"] {
    background: var(--cl-blue-500);
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
                - #[Daily Log](<../Daily Log.md>)
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
            - DNP Modules
                - #[My Daily Notes](<../My Daily Notes.md>) [Your Name](<../Your Name.md>)
                    - ```css
span.rm-page-ref[data-tag="My Daily Notes"] {
	background-image: linear-gradient(to right, var(--cl-gray-600),var(--cl-gray-600));
	background-size: 100%;
    color: var(--cl-white);
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

/*.rm-sidebar-window*/

 span.rm-page-ref[data-tag="My Daily Notes"] + span[data-link-title] {
     background: var(--cl-gray-200) !important;
     color: var(--cl-gray-900) !important;
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
    border-left-color: var(--cl-gray-600);
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="My Daily Notes"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: var(--cl-gray-600);
    border-width: 11px;
    margin-top: -11px;
}```
                - #[Scratchpad](<../Scratchpad.md>)
                    - ```css
span.rm-page-ref[data-tag="Scratchpad"] {
    background: var(--cl-yellow-800);
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Scratchpad"]:before {
    content: '✏️';
}```
                - [Conversation](<../Conversation.md>)
                    - ```css
span.rm-page-ref[data-tag="Conversation"] {
    background: var(--cl-green-700);
    color: var(--cl-white);
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
                - #[Bookmarks](<../Bookmarks.md>)
                    - ```css
span.rm-page-ref[data-tag="Bookmarks"] {
    background: var(--cl-blue-500);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Bookmarks"]:before {
    content: '💾';
}```
                - #[Change Log](<../Change Log.md>)
                    - ```css
span.rm-page-ref[data-tag="Change Log"] {
    background: var(--cl-gray-600);
    color: var(--cl-white);
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
                - #[The Zettelkasten](<../The Zettelkasten.md>)
                    - ```css
span.rm-page-ref[data-tag="The Zettelkasten"] {
    background: var(--cl-gray-600);
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="The Zettelkasten"]:before {
    content: '⚡';
}```
                - [Questions](<../Questions.md>)
                    - ```css
span.rm-page-ref[data-tag="Questions"] {
    background: var(--cl-gray-600);
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Questions"]:before {
    content: '❓';
}```
                - [Promptstorming](<../Promptstorming.md>)
                    - ```css
span.rm-page-ref[data-tag="Promptstorming"] {
    background: var(--cl-red-600);
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Promptstorming"]:before {
    content: '🌪️';
}```
                - #[Help Wanted](<../Help Wanted.md>)
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
                - #[Feedback & Questions](<../Feedback & Questions.md>)
                    - ```css
span.rm-page-ref[data-tag="Feedback & Questions"] {
    background: var(--cl-purple-900);
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Feedback & Questions"]:before {
    content: '📢';
}```
                - "[Questions](<../Questions.md>)"
                - "#[Chat](<../Chat.md>)"
                - #[Dice Roll](<../Dice Roll.md>)
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
            - Notifications & Mentions
                - [@[[Their Name](<../@[[Their Name.md>)]]
                    - Version 1
                        - ```javascript
span[data-link-title^="@"] {
        border: 2px solid [B35555](<../B35555.md>) !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    	line-height: 2em;
} 

span[data-link-title^="@"]:before {
    color: [000746](<../000746.md>) !important;
    content: "🚨unread ";
}

span[data-link-title^="@[Everyone](<../Everyone.md>)"]:before {
    color: [000746](<../000746.md>) !important;
    content: "🚨🚨" !important;
}```
                    - Version 2 [Status](<../Status.md>)/Enabled
                        - ```css
span[data-link-title^="@"] {
  	border:			.5px solid var(--cl-red-700);
    padding: 		2px 5px 2px 5px;
    line-height: 	1em;
    font-weight: 	500;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
	background: 	var(--cl-gray-100);
} 

span[data-link-title^="@"] .rm-page-ref {
  color: var(--cl-red-800) !important;
  font-weight:	600;
}

span[data-link-title^="@"]:before {
    color: 			var(--cl-black);
    content: 		"🚨";
  	padding-right:	3px;
  	font-weight:	300;
  	font-size:		13px;
}

span[data-link-title^="@[Everyone](<../Everyone.md>)"]:before {
    color: var(--cl-black) !important;
    content: "🚨🚨" !important;
}```
                - [cc:[[Their Name](<../cc:[[Their Name.md>)]]
                    - Version 1
                        - ```javascript
span[data-link-title^="cc:"] {
        border: 2px solid [2196F3](<../2196F3.md>) !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="cc:"]:before {
    color: [000746](<../000746.md>) !important;
    content: "📨 ";
}```
                    - Version 2 [Status](<../Status.md>)/Enabled
                        - ```css
span[data-link-title^="cc:"] {
  	border:			.5px solid var(--cl-blue-lt-600);
    padding: 		2px 5px 2px 5px;
    line-height: 	1em;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
	background: 	var(--cl-gray-100);
} 

span[data-link-title^="cc:"] .rm-page-ref {
  color: var(--cl-blue-dk-900) !important;
  font-weight:	600;
}

span[data-link-title^="cc:"]:before {
    color: 			var(--cl-black);
    content: 		"📨";
  	padding-right:	3px;
  	font-weight:	300;
  	font-size:		13px;
}```
                - [~[[Your Name](<../~[[Your Name.md>)]]
                    - Version 1
                        - ```javascript
span[data-link-title^="~"] {
        border: 2px solid [02B920](<../02B920.md>) !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    	line-height: 2em;
} 

span[data-link-title^="~"]:before {
    color: [000746](<../000746.md>) !important;
    content: "✅read "
}```
                    - Version 2 [Status](<../Status.md>)/Enabled
                        - ```css
span[data-link-title^="~"] {
  	border:			.5px solid var(--cl-green-800);
    padding: 		2px 5px 2px 5px;
    line-height: 	1em;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
	background: 	var(--cl-gray-100);
} 

span[data-link-title^="~"] .rm-page-ref {
  color: var(--cl-green-900) !important;
  font-weight:	600;
}

span[data-link-title^="~"]:before {
    color: 			var(--cl-black);
    content: 		"✅";
  	padding-right:	3px;
  	font-weight:	300;
  	font-size:		13px;
}```
                - [^[[Your Name](<../^[[Your Name.md>)]]
                    - Version 1
                        - ```javascript
span[data-link-title^="^"] {
        border: 2px solid [4CAF50](<../4CAF50.md>) !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="^"]:before {
    color: [000746](<../000746.md>) !important;
    content: "💾saved "
}```
                    - Version 2 [Status](<../Status.md>)/Enabled
                        - ```css
span[data-link-title^="^"] {
  	border:			.5px solid var(--cl-gray-800);
    padding: 		2px 5px 2px 5px;
    line-height: 	1em;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
	background: 	var(--cl-gray-100);
} 

span[data-link-title^="^"] .rm-page-ref {
  color: var(--cl-gray-600) !important;
  font-weight:	600;
}

span[data-link-title^="^"]:before {
    color: 			var(--cl-black);
    content: 		"💾";
  	padding-right:	3px;
  	font-weight:	300;
  	font-size:		13px;
}```
            - Note & Zettelkasten Tags
                - #[Fleeting Notes](<../Fleeting Notes.md>)
                    - ```css
span.rm-page-ref[data-tag="Fleeting Notes"] {
	background-image: linear-gradient(45deg, var(--cl-yellow-100), var(--cl-yellow-100));
  	color: [1A1718](<../1A1718.md>) !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - [FN](<../FN.md>)
                    - ```css
/*span.rm-page-ref[data-tag="FN"]:before {
    content: 		'🕊';
}*/

span.rm-page-ref[data-tag="FN"]:after {
    content: 		':';
}

span.rm-page-ref[data-tag="FN"] {
    color: 			var(--cl-gray-900) !important;
    padding: 		2px 5px 2px 5px;
	font-size: 		13px;
    line-height: 	1em;
    font-weight: 	500;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
	background: 	var(--cl-yellow-100);
}```
                - #[Literature Notes](<../Literature Notes.md>)
                    - ```css
span.rm-page-ref[data-tag="Literature Notes"] {
	background-image: linear-gradient(45deg, var(--cl-blue-lt-600), var(--cl-blue-lt-600));
	background-size: 100%;
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - #[LN](<../LN.md>) 
                    - ```css
/*span.rm-page-ref[data-tag="FN"]:before {
    content: 		'🕊';
}*/

span.rm-page-ref[data-tag="LN"]:after {
    content: 		':';
}

span.rm-page-ref[data-tag="LN"] {
    color: 			var(--cl-white) !important;
    padding: 		2px 5px 2px 5px;
	font-size: 		13px;
    line-height: 	1em;
    font-weight: 	500;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
	background: 	var(--cl-blue-lt-600);
}```
                - [Prop](<../Prop.md>)
                    - ```css
span.rm-page-ref[data-tag="Prop"]:after {
    /*content: 		'osition:';*/
  	content: 	":";
}

span.rm-page-ref[data-tag="Prop"] {
    color: 			var(--cl-gray-900) !important;
    padding: 		2px 5px 2px 5px;
	font-size: 		13px;
    line-height: 	1em;
    font-weight: 	500;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
	background: 	var(--cl-yellow-100);
}```
                - #[Seedlings](<../Seedlings.md>)
                    - ```css
span.rm-page-ref[data-tag="Seedlings"] {
	background-image: linear-gradient(90deg, var(--cl-green-300), var(--cl-green-300));
    color: var(--cl-white) !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - #[Buddings](<../Buddings.md>)
                    - ```css
span.rm-page-ref[data-tag="Buddings"] {
	background-image: linear-gradient(90deg, var(--cl-green-600), var(--cl-green-600));
	background-size: 100%;
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - #[Evergreens](<../Evergreens.md>)
                    - ```css
span.rm-page-ref[data-tag="Evergreens"] {
	background-image: linear-gradient(90deg, var(--cl-green-900), var(--cl-green-900));
	background-size: 100%;
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - #[Reference Notes](<../Reference Notes.md>)
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
                - #[Project Ideas](<../Project Ideas.md>)
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
}```
                - #[Annotations](<../Annotations.md>)
                    - ```css
span.rm-page-ref[data-tag="Annotations"] {
	background: [795548](<../795548.md>);
	background-size: 100%;
    color: var(--cl-white);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
                - ### Experimental & Deprecated Note Types
                    - [Evergreen](<../Evergreen.md>)
                        - Tag
                            - ```css
span.rm-page-ref[data-tag="Evergreen"]:before {
    content: '�� '
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
                            - Example: "[Evergreens](<../Evergreens.md>) Prefer note titles with complete phrases to sharpen claims"
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
                    - #[Community Note](<../Community Note.md>) [Test](<../Test.md>)
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
                            - Example: "[Evergreens](<../Evergreens.md>) Prefer note titles with complete phrases to sharpen claims"
                            - ```html
.rm-block-ref > span > span.rm-page-ref--tag[data-tag="Community Notes"]{
  /*display: none;*/
  font-size: .1px;
  line-height: 1.5em;
}

.rm-block-ref > span > span.rm-page-ref--tag[data-tag="Community Note"]:before{
  font-size: 12px;
  margin-right: -5px;
}```
                    - [Notion](<../Notion.md>) [Test](<../Test.md>)
                        - ```css
span.rm-page-ref[data-tag="Notion"]:before {
    content: 		'⛅️ ';
    font-size: 		var(--tag-icon-font-size);
}

span.rm-page-ref[data-tag="Notion"]:after {
    content: 		':';
}

span.rm-page-ref[data-tag="Notion"] {
	color: 			var(--note-tag-color);
 	padding:		var(--note-tag-padding);
/* 	font-weight: 	var(--note-tag-font-weight);*/
  	font-weight:	600;
}```
                    - [Syn](<../Syn.md>) [Test](<../Test.md>)
                        - ```css
span.rm-page-ref[data-tag="Syn"]:before {
    content: 		'🍲 ';
    font-size: 		var(--tag-icon-font-size);
}

span.rm-page-ref[data-tag="Syn"]:after {
    content: 		':';
}

span.rm-page-ref[data-tag="Syn"] {
	color: 			var(--note-tag-color);
 	padding:		var(--note-tag-padding);
/* 	font-weight: 	var(--note-tag-font-weight);*/
  	font-weight:	600;
}```
                    - [Obs](<../Obs.md>) 
                        - ```clojure
span.rm-page-ref[data-tag="Obs"]:before {
    content: 		'🔬 ';
    font-size: 		var(--tag-icon-font-size);
}

span.rm-page-ref[data-tag="Obs"]:after {
    content: 		':';
}

span.rm-page-ref[data-tag="Obs"] {
	color: 			var(--note-tag-color);
 	padding:		var(--note-tag-padding);
 	font-weight: 	var(--note-tag-font-weight);
}```
                    - #[Branching Notes](<../Branching Notes.md>) [Test](<../Test.md>)
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
                    - #[Zettel Questions](<../Zettel Questions.md>)
                        ```css
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
}```
                    - #[Intermediary Notes](<../Intermediary Notes.md>)
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
}```
            - Prepositional Linkages
                - [therefore](<../therefore.md>)
                    - ```css
span.rm-page-ref[data-tag="therefore"]:after {
    content: 		' →';
}

span.rm-page-ref[data-tag="therefore"] {
	color: 			var(--cl-gray-500);
 	padding:		var(--note-tag-padding);
/* 	font-weight: 	var(--note-tag-font-weight);*/
  	font-weight:	600;
}```
            - Block-level Tags
                - #[I](<../I.md>) (Ideas)
                    - ```css
span.rm-page-ref[data-tag="I"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
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
                - [Q](<../Q.md>) (Questions)
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
                - [Ans](<../Ans.md>) (Answers)
                    - ```css
span.rm-page-ref[data-tag="Ans"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Ans"]:before {
    content: '✅'
}```
                - #[Obs](<../Obs.md>) (Observations)
                    - ```css
span.rm-page-ref[data-tag="Obs"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Obs"]:before {
    content: '👀'
}```
                - [G](<../G.md>) (Goals)
                    - ```css
span.rm-page-ref[data-tag="G"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="G"]:before {
    content: '🏆'
}```
            - GTD Tags
                - GTD Core Tags
                    - [INBOX](<../INBOX.md>)
                    - [Inbox](<../Inbox.md>)
                    - [Projects](<../Projects.md>)
                    - [Goals](<../Goals.md>)
                    - #[Agenda](<../Agenda.md>)
                    - #[Follow Up](<../Follow Up.md>)
                    - [Mindsweep](<../Mindsweep.md>)
                    - [Waiting](<../Waiting.md>)
                    - #[Waiting-[[resolved](<../Waiting-[[resolved.md>)]]
                    - [Tracking](<../Tracking.md>)
                    - #[Daily Big 3](<../Daily Big 3.md>)
                    - #[Plan My Day](<../Plan My Day.md>)
                    - #[Weekly Preview](<../Weekly Preview.md>)
                    - #[Next Steps](<../Next Steps.md>)
                    - #[GTD Zone](<../GTD Zone.md>)
                    - Code
                        - ```css
:root {
  --background: var(--cl-gray-600);
  --color: var(--cl-white);
  --padding:2px 5px 2px 5px;
  --font-size: 13px;
  --line-height: 1em;
  --font-weight: 500;
  --border-radius: 5px 5px 5px 5px;
  --position:relative; 
}

span.rm-page-ref[data-tag="GTD Zone"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="GTD Zone"]:before {
    content: '✅';
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

span.rm-page-ref[data-tag="Agenda"] {
    background: var(--background);
    color: var(--color);
    padding: var(--padding);
    font-size: var(--font-size);
    line-height: var(--line-height);
    font-weight: var(--font-weight);
    border-radius: var(--border-radius);
    position: var(--position);
}

span.rm-page-ref[data-tag="Agenda"]:before {
    content: '🗓'
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
                - [Todos](<../Todos.md>)
                    - ```css
span.rm-page-ref[data-tag="Todos"] {
    background: 	var(--cl-yellow-700);
    color: 			var(--cl-white);
    padding: 		2px 5px 2px 5px;
    font-size: 		13px;
    line-height: 	1em;
  	font-weight: 	500;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
}

span.rm-page-ref[data-tag="Todos"]:before {
    content: '🎯';
}```
            - Page-type Tags
                - [Articles](<../Articles.md>)
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
                - [Books](<../Books.md>)
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
                - [Experiments](<../Experiments.md>)
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
                - [Podcasts](<../Podcasts.md>)
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
                - [Tweets](<../Tweets.md>)
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
                - #[Meetings & Discussions](<../Meetings & Discussions.md>)
                    - ```css
span.rm-page-ref[data-tag="Meetings & Discussions"] {
    background: [9E9E9E](<../9E9E9E.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Meetings & Discussions"]:before {
    content: '👥'
}```
                - #[Prompt Ideas](<../Prompt Ideas.md>)
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
                - [Outlines](<../Outlines.md>)
                    - ```css
span.rm-page-ref[data-tag="Outlines"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Outlines"]:before {
    content: '📝'
}```
                - [People](<../People.md>)
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
                - [Members](<../Members.md>)
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
                - [Maxims](<../Maxims.md>)
                    - ```css
span.rm-page-ref[data-tag="Maxims"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Maxims"]:before {
    content: '💫'
}```
                - #[Tips & Tricks](<../Tips & Tricks.md>)
                    - ```css
span.rm-page-ref[data-tag="Tips & Tricks"] {
    background: [9E9E9E](<../9E9E9E.md>);
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
                - [Thoughts](<../Thoughts.md>)
                    - ```css
span.rm-page-ref[data-tag="Thoughts"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Thoughts"]:before {
    content: '💭'
}```
                - [Observations](<../Observations.md>)
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
                - [Conventions](<../Conventions.md>)
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
                - [Processes](<../Processes.md>)
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
                - [Tips](<../Tips.md>)
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
                - Secondary & Experimental
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
                    - `#[Open Questions](<../Open Questions.md>)`
                        - ```html
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
            - Feedback Tags
                - [Feedback](<../Feedback.md>)
                    - #[[[Feedback](<../[[Feedback.md>): What's working]]
                    - #[[[Feedback](<../[[Feedback.md>): What could be better]]
                    - #[[[Feedback](<../[[Feedback.md>): [Suggestions](<../Suggestions.md>)]]
                    - Code
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
                - #[Bug Reports](<../Bug Reports.md>)
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
                - #[Roam Enhancement Requests](<../Roam Enhancement Requests.md>)
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
            - Processing Tags
                - `#[Housekeeping](<../Housekeeping.md>)
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
            - Highlight Tags
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
                - #[My Wins](<../My Wins.md>)
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
                - #[Random Review](<../Random Review.md>)
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
            - Journaling Tags
                - `#[Reflection](<../Reflection.md>)
                    - ```css
span.rm-page-ref[data-tag="Reflection"] {
    background: [607D8B](<../607D8B.md>);
    color: [fff](<../fff.md>);
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Reflection"]:before {
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
            - Status Tags
                - Examples
                    - #[Status/Idea](<../Status/Idea.md>)
                        - ```css
```
                    - #[Status/Active](<../Status/Active.md>)
                        - ```css
```
                    - [Status](<../Status.md>)/On-Hold
                        - ```css
```
                    - #[Status/Dropped](<../Status/Dropped.md>)
                        - ```css
```
                    - [Status](<../Status.md>)/Enabled
                        - ```css
```
                    - [Status](<../Status.md>)/Inactive
                        - ```css
```
                    - [Status](<../Status.md>)/Submitted
                        - ```css
```
                    - [Status](<../Status.md>)/Completed
                        - ```css
```
                    - [Status](<../Status.md>)/Deactivated
                        - ```css
```
                    - #[Status/Someday|Maybe](<../Status/Someday|Maybe.md>)
                        - ```css
```
                    - #[Status/Not Completed](<../Status/Not Completed.md>)
                        - ```css
```
                - Code
                    - ```css
:root {
  --status-padding: 1px 1px 1px 1px;
}

span.rm-page-ref[data-tag="Status/Sent"] {
    background: [03A9F4](<../03A9F4.md>);
    color: [fff](<../fff.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Resolved"] {
    background: [8BC34A](<../8BC34A.md>);
    color: [fff](<../fff.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Closed"] {
    background: [000000](<../000000.md>);
    color: [fff](<../fff.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Completed"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Incomplete"] {
    color: [607D8B](<../607D8B.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Waiting-For"] {
    color: [795548](<../795548.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/On-Hold"] {
    color: [6A6A6A](<../6A6A6A.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Dropped"] {
    color: [C30D00](<../C30D00.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Active"] {
    color: [2196F3](<../2196F3.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Approved"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Someday|Maybe"] {
    color: [467C96](<../467C96.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Not-Completed, Carried"] {
    color: [FF9800](<../FF9800.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Enabled"] {
    color: [4CAF50](<../4CAF50.md>);
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            - Miscellaneous
                - `#[Quick Capture](<../Quick Capture.md>)
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
                - `[Problems](<../Problems.md>)
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
            - Experimental
                - `[Quote](<../Quote.md>) (inline block ref)
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
                - [Personas](https://www.rodrigofranco.com/roam-personas-css.html) [Experiments](<../Experiments.md>)
                    - Examples
                        - #[P:Self](<../P:Self.md>) Inner Self Talk
                        - #[P:Loving](<../P:Loving.md>) Love thyself
                        - #[P:Critic](<../P:Critic.md>) Hard on yourself
                    - Code
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
            - Archived & Deprecated
                - Depreciated
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
                    - `[Reply-from](<../Reply-from.md>) [your_name_here](<../your_name_here.md>)`
                        - ```html
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
                    - `#[Posted by](<../Posted by.md>) [your_name_here](<../your_name_here.md>)`
                    - [Help](<../Help.md>) [your_name_here](<../your_name_here.md>)
                        - ```html
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
                    - #@ [your_name_here](<../your_name_here.md>)
                        - ```html
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
                - `[Resolved](<../Resolved.md>)`
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
                - `[Happenings](<../Happenings.md>)`
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
                - `[Disabled](<../Disabled.md>)`
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
                - `[Important](<../Important.md>)`
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
                - `[Urgent](<../Urgent.md>)`
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
                - `Alert/ tags`
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
                - `[Flag](<../Flag.md>)`
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
                - `Flag/ tags`
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
                - `SCC/ tags`
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
                - `#[Focus Mode (plus)](<../Focus Mode (plus).md>)`
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
                - `#[Action Items](<../Action Items.md>)`
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
                - `Evergreen tags` ([Legacy](<../Legacy.md>))
                    - ```html
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
        - User Interface
            - Buttons & Word Count [Status](<../Status.md>)/Enabled
                - Example: {{word-count}}
                - Code
                    - ```css
/* Buttons in Block Text */
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-block-text > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: var(--cl-gray-200);
  color:			var(--cl-gray-700);
  font-size: 		11px;
  line-height: 		13px;
  padding: 			2px 4px 2px 4px; 
  min-height: 		0px;
}

/* Buttons in Block References */
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-block-ref > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: var(--cl-gray-200);
  color:			var(--cl-gray-700);
  font-size: 		11px;
  line-height: 		13px;
  padding: 			2px 4px 2px 4px; 
  min-height: 		0px;
}

/* Buttons in Zoom Masks */
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]),
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]):focus,
.rm-zoom-item > span > div > div > span > .bp3-button:not([class*="bp3-intent-"]):hover {
  background-color: var(--cl-gray-200);
  color:			var(--cl-gray-700);
  font-size: 		11px;
  line-height: 		13px;
  padding: 			2px 4px 2px 4px; 
  min-height: 		0px;
}```
            - Scope Highlighting ((This colors the vertical lines to show your mouse location and the bullet that you are editing)) [Status](<../Status.md>)/Enabled
                - ```css

.roam-block-container  div.roam-block-container {
box-shadow: -2px 0px var(--cl-gray-600));
transition: box-shadow 1s;
}

.roam-block-container div.roam-block-container:hover {
box-shadow: -0.5px 0px var(--cl-gray-800);
transition:  box-shadow 0.5s;
}

.roam-block-container:focus-within > .rm-block-main > div:nth-child(1) 
.rm-bullet .rm-bullet__inner  
{
background-color: var(--cl-black);
}```
            - Query Display Options [Status](<../Status.md>)/Enabled
                - Code
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

[data-tag="min-all"] + .rm-query .zoom-mentions-view,
[data-tag="min-all"] + .rm-query .rm-title-arrow-wrapper,
[data-tag="min-all"] + .rm-query .rm-query-title {
  display:none !important;  /* hide everything */
}

span [data-tag="min-all"] {
  display: 			none;
  height: 			0px !important;
  max-height:		0px !important;
  line-height:		0px !important;
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
            - Prevent right sidebar title from jumping around when editing [Status](<../Status.md>)/Enabled
                - ```css

[right-sidebar](<../right-sidebar.md>) .rm-title-textarea {
    width: 95%;
}```
            - Show Main Page multibar [Status](<../Status.md>)/Enabled
                - This is to stop people (read: me :P ) from accidentally clicking on the bar
                - ```css

.rm-level-0>.rm-multibar {
    opacity: .3;
  	border-right: 1px dashed [BFCCD6](<../BFCCD6.md>), .2) !important;
}
.rm-level-0>.rm-multibar:hover {
    border-right: 3px solid [5C7080](<../5C7080.md>), .5);
}```
            - Left Sidebar — Highlight important pages [Status](<../Status.md>)/Enabled
                - ```css

.starred-pages a[href*="MorTyZR-2"]>.page,
.starred-pages a[href*="sQPmakIfe"]>.page,
.starred-pages a[href*="TxsV9GIET"]>.page
{
  color: [FFCF40](<../FFCF40.md>) !important;
}

.starred-pages a[href*="S04orQeHK"]>.page,
.starred-pages a[href*="9QGedI_a3"]>.page,
.starred-pages a[href*="vxKXH9a0r"]>.page
{
  color: [2196F3](<../2196F3.md>) !important;
}

.starred-pages a[href*="ohDe4FbVt"]>.page,
.starred-pages a[href*="7CWEj1_kU"]>.page,
.starred-pages a[href*="7y86LvOF6"]>.page
{
  color: [9E9E9E](<../9E9E9E.md>) !important;
}```
            - Breaks — `---`
                - ---
                    - ```css
.rm-hr {
  border: 			.25px dashed var(--cl-gray-500);
  margin-bottom: 	10px;
}```
        - Content
            - Headings [Status](<../Status.md>)/Enabled
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
  --fnt-size-h1:       		20px;
  --fnt-size-h2:       		17px;
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
            - Page References [Status](<../Status.md>)/Enabled
                - ```css
.rm-page-ref-link-color {
    color: var(--cl-blue-500);
    font-weight: 400;
}

a {
    color: var(--cl-blue-500);
}```
            - Page Reference Brackets
                - ```ruby
.rm-page-ref__brackets{
  display:none;
}```
            - Block Reference styling [Status](<../Status.md>)/Enabled
                - ```css
/*Block Reference formatting*/

.rm-block-ref {
    font-weight: 390;
  	font-style: italic;
    /*color: [009688](<../009688.md>);
  	text-decoration: underline;
  	text-decoration-color: [FF9800](<../FF9800.md>); */
}```
            - Page Reference Underlines & Nested Links [Status](<../Status.md>)/Enabled
                - Example
                    - [Evergreens/active vs passive resurfacing](<../Evergreens/active vs passive resurfacing.md>)
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
    padding-bottom: 2px;
/*    line-height: 28px;*/
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
            - External Links [Status](<../Status.md>)/Enabled
                - V1
                    - ```css
.rm-alias--external {
  color: var(--fg-link);
}

.rm-alias--external:after {
  content: '↗';
}

.rm-alias--external:hover {
    text-decoration: none!important;
    border-bottom: 1px dashed;
    color: var(--cl-blue-900);
}
  
.rm-alias--external{
  color: var(--cl-blue-700);
  text-decoration: none!important;
  border-bottom: 1px solid;
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
            - Spacing
                - Spacing using `[ubrk](<../ubrk.md>)` (up break) & `[dbrk](<../dbrk.md>)` (down break)
                    - ```css
[data-page-links="dbrk"] > .rm-block-main { 
    margin-bottom: 1em !important;
}

span.rm-page-ref[data-tag="dbrk"] {
  display: none;
}

[data-page-links*="ubrk"] > .rm-block-main { 
    margin-top: .25em !important;
}

span.rm-page-ref[data-tag="ubrk"] {
  display: none;
}```
            - Block Highlightings
                - Block Highlights
                    - `[blk-gray](<../blk-gray.md>)` [blk-gray](<../blk-gray.md>)
                        - ```css
[data-page-links*="blk-gray"] > .rm-block-main {
    /* color: [383d41](<../383d41.md>); */
    background-color: var(--cl-gray-200);
    border: .5px dashed var(--cl-gray-400); 
    /*margin-bottom: 5px;*/
}

span.rm-page-ref[data-tag="blk-gray"] {
  display: none;
}```
        - Miscellaneous
            - Sign Up Form Iframe
                - ```css
iframe[src*="docs.google.com"] {
  height: 1100px;
}```
    - Patch Fixes
        - Fix for orange blocks ((Unsure purpose - BT))
            - ```css
[find-or-create-input](<../find-or-create-input.md>) {
   outline: none!important;
}```
    - Archive
        - Left side-bar 
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
        - Headings & font
            - ```clojure
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
}```

# Backlinks
## [Agenda](<Agenda.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [CSS](<CSS.md>)
- **[Redirect](<../Redirect.md>):** [roam/css](<../roam/css.md>)

## [Decisions](<Decisions.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [Development Requests](<Development Requests.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [Drafts](<Drafts.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [February 10th, 2021](<February 10th, 2021.md>)
- {{[query](<../query.md>): {and: [Agenda](<../Agenda.md>) {not: [roam/css](<../roam/css.md>)]

## [February 22nd, 2021](<February 22nd, 2021.md>)
- [min-con](<../min-con.md>) {{[query](<../query.md>): {and: [Help Wanted](<../Help Wanted.md>) [TODO](<../TODO.md>){not: {or: [DONE](<../DONE.md>) [roam/css](<../roam/css.md>)}

## [February 23rd, 2021](<February 23rd, 2021.md>)
- [min-con](<../min-con.md>) {{[query](<../query.md>): {and: [Help Wanted](<../Help Wanted.md>) [TODO](<../TODO.md>) {not: {or: [DONE](<../DONE.md>) [roam/css](<../roam/css.md>)}

## [February 2nd, 2021](<February 2nd, 2021.md>)
- (resolved) "[Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

## [Frameworks](<Frameworks.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [Graph/Templates](<Graph/Templates.md>)
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

- [minimal](<../minimal.md>) {{[query](<../query.md>): {and: [Evergreens](<../Evergreens.md>) {not: {or: [E:](<../E:.md>) [roam/css](<../roam/css.md>)}

## [January 31st, 2021](<January 31st, 2021.md>)
- "[Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

- [Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

10. "Yup " — "[Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

- "[Q](<../Q.md>) Is it possible to change [roam/css](<../roam/css.md>)

## [Members](<Members.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [Outlines](<Outlines.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

## [People](<People.md>)
- [x] Add to [roam/css](<../roam/css.md>)

## [Thoughts](<Thoughts.md>)
- [ ] Add to [roam/css](<../roam/css.md>)

