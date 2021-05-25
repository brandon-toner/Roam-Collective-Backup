- **[Tags](<../Tags.md>):** [Seedpack](<../Seedpack.md>)
    - **[Created by](<../Created by.md>):** [Charles Farr](<../Charles Farr.md>)
    - **[Date Created](<../Date Created.md>):** [March 18th, 2021](<../March 18th, 2021.md>)
    - ---
    - Welcome
        - Welcome! With this single page, you will be able to quickly get your graph set up and your adventure underway.
        - As you work through the graph, feel free to import portions of the conventions, styling, and code.
        - The below guide assumes that you have some familiarity with Roam. If you are a completely new user, the following are useful resources to get up to speed:
            - [ ] Add tutorial references
        - Please review this quick video explaining how to integrate this seedpack into your graph.
            - [ ] Add video illustrating the approach
    - Templates
        - [ ] Add templates for general pages, css page structure
    - Creation of Core Pages
        - Functional Pages
            - [roam/js](<../roam/js.md>)
            - [roam/css](<../roam/css.md>)
        - Organizational Pages
            - [Graph/Templates](<../Graph/Templates.md>)
            - [Graph/SmartBlocks](<../Graph/SmartBlocks.md>)
            - [Graph/Extensions](<../Graph/Extensions.md>)
        - Information Pages
            - [Onboarding/Using conventions](<../Onboarding/Using conventions.md>)
            - [Onboarding/Using extensions](<../Onboarding/Using extensions.md>)
    - Importing Key Functions
        - Roam42
            - **[Info](<../Info.md>):**
                - Roam42 is a javascript extension for Roam Research, adding some incredibly powerful features.
                - For more information on Roam42, see [Roam42.com](https://roam42.com)
            - **[Import Instructions](<../Import Instructions.md>):**
                - Drag the Roam42 js block below into the [Graph/Extensions](<../Graph/Extensions.md>) page
                - Drag the Roam42 Conventions & Uses below into the [Onboarding/Using extensions](<../Onboarding/Using extensions.md>) page
            - Roam42 js
                - {{{[roam/js](<../roam/js.md>)}}}
                    - ```javascript
{
var s = document.createElement('script');
	s.type = "text/javascript";
  	s.src =  "https://roam42.glitch.me/main.js";
  	s.async = true;
document.body.appendChild(s);
}```
            - Roam42 Conventions & Uses
                - [ ] Add overview of Roam42
                - [ ] Link to later SmartBlocks section
        - Color Scheme
            - **[Info](<../Info.md>):**
                - The following CSS uses a standard color scheme to style elements. All of the CSS code here draws on the color scheme.
            - **[Import Instructions](<../Import Instructions.md>):**
                - Drag either the Color Scheme (Hosted) or the Color Scheme (Full) into the [roam/css](<../roam/css.md>) page
            - **[Code](<../Code.md>):**
                - Color Scheme (Hosted)
                    - ```css
/* Standard color scheme from Roam Collective */

@import url("https://raw.githubusercontent.com/roam-collective/color-schemes/main/color-schemes/standard.css");```
                    - For additional color schemes and information, see the [RC repo](https://github.com/roam-collective/color-schemes/tree/main/color-schemes)
                    - [ ] Fix the above `@import` statement...
                - Color Scheme (Full)
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
  --cl-blue-dk-900: [263a83ff](<../263a83ff.md>); /* --dark-cornflower-blue-2:  */
}```
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
        - Optional UI Tweaks
            - [ ] Add or delete...
            - Query Views
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
[data-tag="min-q"] + .rm-query .rm-query-title,
[data-tag="min-con"] + .rm-query .rm-query-title {
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
            - Line Breaks `---`
                - ---
                    - ```css
.rm-hr {
  border: 			.5px dashed var(--cl-gray-500);
  margin: 	10px 0px 10px 0px;
}```
    - Importing Conventions
        - Daily Notes Modules
            - **[Info](<../Info.md>):**
                - 
            - **[Import Instructions](<../Import Instructions.md>):**
            - **[Code](<../Code.md>):**
                - #[My Daily Notes](<../My Daily Notes.md>) [Your Name](<../Your Name.md>)
                    - ```css
span.rm-page-ref[data-tag="My Daily Notes"] 
{ 
  background: 		var(--cl-gray-300);
  color: 			var(--cl-black);
  padding: 			2px 5px 2px 5px;
  font-size: 		13px;
  line-height: 		1rem;
  font-weight: 		600;
  border-radius: 	5px 5px 5px 5px;
  border-style: 	solid;
  border-color: 	var(--cl-gray-800);
  border-width: 	thin;
  position:			relative;
  box-shadow: 		0px 1px 3px -1px var(--cl-black), 0px -1px 3px  var(--cl-gray-500);
  z-index:			1;
}

span.rm-page-ref[data-tag="My Daily Notes"] + span[data-link-title] 
{
  	background: 	var(--cl-white);
  	font-size: 		13px;
  	line-height: 	1rem;
  	border-radius: 	5px 5px 5px 5px;
  	border-style: 	solid;
  	border-color: 	var(--cl-gray-800);
  	border-width: 	thin;
    border-radius: 	0 5px 5px 0;
	margin-left: 	-10px;
  	padding: 		2px 5px 2px 15px;
  	position:		relative;
  	box-shadow: 	0px 1px 3px -1px var(--cl-black), 0px -1px 3px  var(--cl-gray-500);
  	z-index:		-1;
}

span.rm-page-ref[data-tag="My Daily Notes"] + span[data-link-title] > .rm-page-ref
{
  	color: 			var(--cl-yellow-900);
  	font-weight:	500;
}```
                - [Scratchpad](<../Scratchpad.md>)
                    - ```css
span.rm-page-ref[data-tag="Scratchpad"] 
{ background: 		var(--cl-white);
  background-size: 	100%;
  color: 			var(--cl-black);
  padding: 			2px 5px 2px 5px;
  font-size: 		13px;
  line-height: 		1rem;
  font-weight: 		500;
  border-radius: 	5px 5px 5px 5px;
  border-style: 	solid;
  border-color: 	var(--cl-gray-800);
  border-width: 	thin;
  position:			relative;
  box-shadow: 		0px 1px 3px -1px var(--cl-black), 0px -1px 3px  var(--cl-gray-500);
}

span.rm-page-ref[data-tag="Scratchpad"]:before {
    content: 		'✏️';
  	padding-right:	2px;
}```
                - #[Conversation & Comments](<../Conversation & Comments.md>)
                    - ```css
span.rm-page-ref[data-tag="Conversation"] 
{ background: 		var(--cl-white);
  background-size: 	100%;
  color: 			var(--cl-black);
  padding: 			2px 5px 2px 5px;
  font-size: 		13px;
  line-height: 		1rem;
  font-weight: 		500;
  border-radius: 	5px 5px 5px 5px;
  border-style: 	solid;
  border-color: 	var(--cl-gray-800);
  border-width: 	thin;
  position:			relative;
  box-shadow: 		0px 1px 3px -1px var(--cl-black), 0px -1px 3px  var(--cl-gray-500);
}

span.rm-page-ref[data-tag="Conversation"]:before {
    content: 		'📮';
  	padding-right: 	2px;
}```
                - [Todos](<../Todos.md>)
                    - ```css
span.rm-page-ref[data-tag="Todos"] 
{ background: 		var(--cl-white);
  background-size: 	100%;
  color: 			var(--cl-black);
  padding: 			2px 5px 2px 5px;
  font-size: 		13px;
  line-height: 		1rem;
  font-weight: 		500;
  border-radius: 	5px 5px 5px 5px;
  border-style: 	solid;
  border-color: 	var(--cl-gray-800);
  border-width: 	thin;
  position:			relative;
  box-shadow: 		0px 1px 3px -1px var(--cl-black), 0px -1px 3px  var(--cl-gray-500);
}

span.rm-page-ref[data-tag="Todos"]:before {
    content: 		'🎯';
  	padding-right: 	2px;
}```
                - #[Change Log](<../Change Log.md>)
                    - ```css
span.rm-page-ref[data-tag="Change Log"] 
{ background: 		var(--cl-white);
  background-size: 	100%;
  color: 			var(--cl-black);
  padding: 			2px 5px 2px 5px;
  font-size: 		13px;
  line-height: 		1rem;
  font-weight: 		500;
  border-radius: 	5px 5px 5px 5px;
  border-style: 	solid;
  border-color: 	var(--cl-gray-800);
  border-width: 	thin;
  position:			relative;
  box-shadow: 		0px 1px 3px -1px var(--cl-black), 0px -1px 3px  var(--cl-gray-500);
}

span.rm-page-ref[data-tag="Change Log"]:before {
    content: '📢';
  	padding-right: 2px;  
}```
            - Using the My Daily Notes section in a multiplayer graph 
        - Communication
            - **[Info](<../Info.md>):**
            - **[Import Instructions](<../Import Instructions.md>):**
            - **[Code](<../Code.md>):**
                - [@[[Their Name](<../@[[Their Name.md>)]]
                    - ```css
span[data-link-title^="@"] .rm-page-ref {
  color: 			var(--cl-orange-600);
  font-weight:		500;
}

/*span[data-link-title^="@"]:before {
  	padding-right:	3px;
  	font-weight:	300;
  	font-size:		13px;
}*/

span[data-link-title^="@[Admin](<../Admin.md>)"]:before {
    color: 			var(--cl-black) !important;
    content: 		"🚨🚨" !important;
}```
                - [cc:[[Their Name](<../cc:[[Their Name.md>)]]
                    - ```css
span[data-link-title^="cc:"] .rm-page-ref {
  color: 			var(--cl-yellow-800) !important;
  font-weight:		500;
}

/*span[data-link-title^="cc:"]:before {
    color: 			var(--cl-black);
  	padding-right:	3px;
  	font-weight:	300;
  	font-size:		13px;
}*/```
                - [~[[Your Name](<../~[[Your Name.md>)]]
                    - ```css
span[data-link-title^="~"] .rm-page-ref {
  color: var(--cl-green-900) !important;
  font-weight:	500;
}

/*span[data-link-title^="~"]:before {
    color: 			var(--cl-black);
   	content: 		"✅";
  	padding-right:	3px;
  	font-weight:	300;
  	font-size:		13px;
}*/```
                - [^[[Your Name](<../^[[Your Name.md>)]]
                    - ```css
span[data-link-title^="^"] .rm-page-ref {
  color: 			var(--cl-blue-600) !important;
  font-weight:		500;
}```
            - Using the communication tags within a multiplayer graph
        - Notes & Questions
            - **[Info](<../Info.md>):**
            - **[Import Instructions](<../Import Instructions.md>):**
            - **[Code](<../Code.md>):**
                - [Q](<../Q.md>) → Questions
                    - ```css
span.rm-page-ref[data-tag="Q"] {
    color: 			var(--cl-purple-800);
    font-weight: 	600;
}
span.rm-page-ref[data-tag="Q"]:after {
    content: 		':';
}```
                - [I](<../I.md>) → Ideas
                    - ```css
span.rm-page-ref[data-tag="I"] {
    color: 			var(--cl-yellow-900);
    font-weight: 	600;
}
span.rm-page-ref[data-tag="I"]:after {
    content: 		':';
}```
                - [N](<../N.md>) → Note to resurface
                    - ```css
span.rm-page-ref[data-tag="N"] {
    color: 			var(--cl-green-900);
    font-weight: 	600;
}
span.rm-page-ref[data-tag="N"]:after {
    content: 		':';
}```
            - Capturing notes & questions within a multiplayer graph
        - Page Structures
            - **[Info](<../Info.md>):**
            - **[Import Instructions](<../Import Instructions.md>):**
            - **[Code](<../Code.md>):**
                - [ ] Pull in templates
        - Task Management
            - Add
    - Importing Dashboards
        - 
    - Building on the Primitives
    - Clean Up
        - [ ] Delete any start up templates

# Backlinks
## [March 18th, 2021](<March 18th, 2021.md>)
- Working on a combo seedpack / onboarding package → [RC/Onboarding Seedpack](<../RC/Onboarding Seedpack.md>)

## [March 20th, 2021](<March 20th, 2021.md>)
- Fiddling with [RC/Onboarding Seedpack](<../RC/Onboarding Seedpack.md>)

