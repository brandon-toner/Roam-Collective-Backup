- Tags:: #Seedpack
    - Created by:: [[Charles Farr]]
    - Date Created:: [[March 18th, 2021]]
    - ---
    - Welcome
        - Welcome! With this single page, you will be able to quickly get your graph set up and your adventure underway.
        - As you work through the graph, feel free to import portions of the conventions, styling, and code.
        - The below guide assumes that you have some familiarity with Roam. If you are a completely new user, the following are useful resources to get up to speed:
            - {{[[TODO]]}} Add tutorial references
        - Please review this quick video explaining how to integrate this seedpack into your graph.
            - {{[[TODO]]}} Add video illustrating the approach
    - Templates
        - {{[[TODO]]}} Add templates for general pages, css page structure
    - Creation of Core Pages
        - Functional Pages
            - [[roam/js]]
            - [[roam/css]]
        - Organizational Pages
            - [[Graph/Templates]]
            - [[Graph/SmartBlocks]]
            - [[Graph/Extensions]]
        - Information Pages
            - [[Onboarding/Using conventions]]
            - [[Onboarding/Using extensions]]
    - Importing Key Functions
        - Roam42
            - Info::
                - Roam42 is a javascript extension for Roam Research, adding some incredibly powerful features.
                - For more information on Roam42, see [Roam42.com](https://roam42.com)
            - Import Instructions::
                - Drag the Roam42 js block below into the [[Graph/Extensions]] page
                - Drag the Roam42 Conventions & Uses below into the [[Onboarding/Using extensions]] page
            - Roam42 js
                - {{{[[roam/js]]}}}
                    - ```javascript
{
var s = document.createElement('script');
	s.type = "text/javascript";
  	s.src =  "https://roam42.glitch.me/main.js";
  	s.async = true;
document.body.appendChild(s);
}```
            - Roam42 Conventions & Uses
                - {{[[TODO]]}} Add overview of Roam42
                - {{[[TODO]]}} Link to later SmartBlocks section
        - Color Scheme
            - Info::
                - The following CSS uses a standard color scheme to style elements. All of the CSS code here draws on the color scheme.
            - Import Instructions::
                - Drag either the Color Scheme (Hosted) or the Color Scheme (Full) into the [[roam/css]] page
            - Code::
                - Color Scheme (Hosted)
                    - ```css
/* Standard color scheme from Roam Collective */

@import url("https://raw.githubusercontent.com/roam-collective/color-schemes/main/color-schemes/standard.css");```
                    - For additional color schemes and information, see the [RC repo](https://github.com/roam-collective/color-schemes/tree/main/color-schemes)
                    - {{[[TODO]]}} Fix the above `@import` statement...
                - Color Scheme (Full)
                    - Black, White, Gray
                        - ```css
:root {
  --cl-white:    #ffffff;
  --cl-gray-100: #f8f9faff; /*--cultured*/
  --cl-gray-200: #e9ecefff; /*--cultured-2*/
  --cl-gray-300: #dee2e6ff; /*--gainsboro*/
  --cl-gray-400: #ced4daff; /*--light-gray*/
  --cl-gray-500: #adb5bdff; /*--cadet-blue-crayola*/
  --cl-gray-600: #6c757dff; /*--slate-gray*/
  --cl-gray-700: #495057ff; /*--davys-grey*/
  --cl-gray-800: #343a40ff; /*--gunmetal*/
  --cl-gray-900: #212529ff; /*--charleston-green*/
  --cl-black:    #000000;
}```
                    - Red
                        - ```css
:root {
  --cl-red-100: #ffc2c4ff; /*--spanish-pink*/
  --cl-red-200: #f9acafff; /*--light-pink*/
  --cl-red-300: #f3969aff; /*--salmon-pink*/
  --cl-red-400: #ed8084ff; /*--light-coral*/
  --cl-red-500: #e86b6fff; /*--candy-pink*/
  --cl-red-600: #e2555aff; /*--indian-red*/
  --cl-red-700: #dc3f45ff; /*--rose-madder*/
  --cl-red-800: #d6292fff; /*--amaranth-red*/
  --cl-red-900: #d0131aff; /*--lava*/
}```
                    - Orange
                        - ```css
:root {
  --cl-orange-100: #ffcdadff; /*--apricot:*/
  --cl-orange-200: #fbbe97ff; /*--peach-crayola:*/
  --cl-orange-300: #f7af82ff; /*--macaroni-and-cheese:*/
  --cl-orange-400: #f3a06cff; /*--atomic-tangerine:*/
  --cl-orange-500: #f09257ff; /*--atomic-tangerine-2:*/
  --cl-orange-600: #ec8341ff; /*--princeton-orange:*/
  --cl-orange-700: #e8742bff; /*--spanish-orange:*/
  --cl-orange-800: #e46516ff; /*--spanish-orange-2:*/
  --cl-orange-900: #e05600ff; /*--persimmon:*/
}```
                    - Yellow
                        - ```css
:root {
  --cl-yellow-100: #FDEAB4ff; /*--jasmine:*/
  --cl-yellow-200: #fbdc86ff; /*--jasmine-2:*/
  --cl-yellow-300: #f7d473ff; /*--orange-yellow-crayola:*/
  --cl-yellow-400: #f3cc60ff; /*--maize-crayola:*/
  --cl-yellow-500: #f0c54dff; /*--maize-crayola-2:*/
  --cl-yellow-600: #ecbd39ff; /*--saffron:*/
  --cl-yellow-700: #e8b526ff; /*--orange-yellow:*/
  --cl-yellow-800: #e4ad13ff; /*--goldenrod:*/
  --cl-yellow-900: #e0a500ff; /*--goldenrod-2:*/

}```
                    - Green Yellow
                        - ```css
:root {
  --cl-green-yel-100: #eaecacff;/*--pale-spring-bud:*/
  --cl-green-yel-200: #e1e39bff;/*--green-yellow-crayola:*/
  --cl-green-yel-300: #d8da8bff;/*--khaki-x-11-light-khaki:*/
  --cl-green-yel-400: #cfd17aff;/*--straw:*/
  --cl-green-yel-500: #c6c96aff;/*--dark-khaki:*/
  --cl-green-yel-600: #bcc059ff;/*--olive-green:*/
  --cl-green-yel-700: #b3b748ff;/*--olive-green-2:*/
  --cl-green-yel-800: #aaae38ff;/*--citron:*/
  --cl-green-yel-900: #a1a527ff;/*--citron-2:*/
}```
                    - Green
                        - ```css
:root {
  --cl-green-100: #cae4a0ff; /*--yellow-green-crayola:*/
  --cl-green-200: #bed991ff; /*--yellow-green-crayola-2:*/
  --cl-green-300: #b2cf82ff; /*--pistachio:*/
  --cl-green-400: #a5c473ff; /*--olivine:*/
  --cl-green-500: #99ba64ff; /*--olivine-2:*/
  --cl-green-600: #8daf55ff; /*--olivine-3:*/
  --cl-green-700: #81a446ff; /*--moss-green:*/
  --cl-green-800: #749a37ff; /*--olive-drab-3:*/
  --cl-green-900: #688f28ff; /*--olive-drab-3-2:*/
}```
                    - Green-Blue
                        - ```css
:root {
  --cl-green-blu-100: #a8dcd9ff;/*--powder-blue:*/ 
  --cl-green-blu-200: #9ad3d0ff;/*--middle-blue-green:*/ 
  --cl-green-blu-300: #8dc9c6ff;/*--middle-blue-green-2:*/ 
  --cl-green-blu-400: #7fc0bdff;/*--green-sheen:*/ 
  --cl-green-blu-500: #72b7b3ff;/*--green-sheen-2:*/ 
  --cl-green-blu-600: #64adaaff;/*--verdigris:*/ 
  --cl-green-blu-700: #56a4a0ff;/*--cadet-blue:*/ 
  --cl-green-blu-800: #499a97ff;/*--cadet-blue-2:*/ 
  --cl-green-blu-900: #3b918dff;/*--viridian-green:*/ 
}```
                    - Blue (lighter shade)
                        - ```css
:root {
  --cl-blue-lt-100: #aec7efff; /*--baby-blue-eyes:*/
  --cl-blue-lt-200: #a0bce9ff; /*--baby-blue-eyes-2:*/
  --cl-blue-lt-300: #8fafe2ff; /*--french-sky-blue:*/
  --cl-blue-lt-400: #7ea5e0ff; /*--little-boy-blue:*/
  --cl-blue-lt-500: #7099daff; /*--cornflower-blue:*/
  --cl-blue-lt-600: #5f8cd3ff; /*--united-nations-blue:*/
  --cl-blue-lt-700: #4c7eceff; /*--glaucous:*/
  --cl-blue-lt-800: #3770cbff; /*--celtic-blue:*/
  --cl-blue-lt-900: #2b66c4ff; /*--true-blue:*/}```
                    - Blue
                        - ```css
:root {
  --cl-blue-100:   #dceff9ff; /*--alice-blue:*/
  --cl-blue-200:   #a7d9f1ff; /*--uranian-blue:*/
  --cl-blue-300:   #85c6e9ff; /*--light-cornflower-blue:*/
  --cl-blue-400:   #5aaddcff; /*--blue-jeans:*/
  --cl-blue-500:   #389bd5ff; /*--carolina-blue:*/
  --cl-blue-600:   #1e7ac0ff; /*--star-command-blue:*/
  --cl-blue-700:   #0254a0ff; /*--usafa-blue:*/
  --cl-blue-800:   #014889ff; /*--yale-blue:*/
  --cl-blue-900:   #023a72ff; /*--indigo-dye:*/
}```
                    - Blue (Darker Shade)
                        - ```css
:root {
  --cl-blue-dk-100: #7a8fd8ff; /* --cornflower-blue:  */
  --cl-blue-dk-200: #6e85d0ff; /* --glaucous:  */
  --cl-blue-dk-300: #6076c9ff; /* --han-blue:  */
  --cl-blue-dk-400: #526cc1ff; /* --han-blue-2:  */
  --cl-blue-dk-500: #455eb9ff; /* --liberty:  */
  --cl-blue-dk-600: #3f56aaff; /* --cerulean-blue:  */
  --cl-blue-dk-700: #3a4f99ff; /* --y-in-mn-blue:  */
  --cl-blue-dk-800: #30448fff; /* --dark-cornflower-blue:  */
  --cl-blue-dk-900: #263a83ff; /* --dark-cornflower-blue-2:  */
}```
                    - Violet
                        - ```css
:root {
  --cl-violet-100: #afb1d4ff; /*--wild-blue-yonder*/
  --cl-violet-200: #a2a4caff; /*--blue-bell*/
  --cl-violet-300: #9597c0ff; /*--blue-bell-2*/
  --cl-violet-400: #888ab6ff; /*--cool-grey*/
  --cl-violet-500: #7b7eadff; /*--rhythm*/
  --cl-violet-600: #6e71a3ff; /*--dark-blue-gray*/
  --cl-violet-700: #616499ff; /*--dark-blue-gray-2*/
  --cl-violet-800: #54578fff; /*--purple-navy*/
  --cl-violet-900: #474a85ff; /*--purple-navy-2*/
}```
                    - Purple
                        - ```css
:root {
  --cl-purple-100: #bfaed5ff; /*--lilac*/
  --cl-purple-200: #b3a1cbff; /*--glossy-grape*/
  --cl-purple-300: #a894c2ff; /*--glossy-grape-2*/
  --cl-purple-400: #9c87b8ff; /*--purple-mountain-majesty*/
  --cl-purple-500: #907aaeff; /*--purple-mountain-majesty-2*/
  --cl-purple-600: #846ca4ff; /*--middle-blue-purple*/
  --cl-purple-700: #795f9bff; /*--royal-purple*/
  --cl-purple-800: #6d5291ff; /*--royal-purple-2*/
  --cl-purple-900: #614587ff; /*--cyber-grape*/
}```
        - Optional UI Tweaks
            - {{[[TODO]]}} Add or delete...
            - Query Views
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
            - Line Breaks `---`
                - ---
                    - ```css
.rm-hr {
  border: 			.5px dashed var(--cl-gray-500);
  margin: 	10px 0px 10px 0px;
}```
    - Importing Conventions
        - Daily Notes Modules
            - Info::
                - 
            - Import Instructions::
            - Code::
                - #[[My Daily Notes]] [[Your Name]]
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
                - #Scratchpad
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
                - #[[Conversation & Comments]]
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
                - #Todos
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
                - #[[Change Log]]
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
            - Info::
            - Import Instructions::
            - Code::
                - [[@[[Their Name]]]]
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

span[data-link-title^="@[[Admin]]"]:before {
    color: 			var(--cl-black) !important;
    content: 		"🚨🚨" !important;
}```
                - [[cc:[[Their Name]]]]
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
                - [[~[[Your Name]]]]
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
                - [[^[[Your Name]]]]
                    - ```css
span[data-link-title^="^"] .rm-page-ref {
  color: 			var(--cl-blue-600) !important;
  font-weight:		500;
}```
            - Using the communication tags within a multiplayer graph
        - Notes & Questions
            - Info::
            - Import Instructions::
            - Code::
                - #Q → Questions
                    - ```css
span.rm-page-ref[data-tag="Q"] {
    color: 			var(--cl-purple-800);
    font-weight: 	600;
}
span.rm-page-ref[data-tag="Q"]:after {
    content: 		':';
}```
                - #I → Ideas
                    - ```css
span.rm-page-ref[data-tag="I"] {
    color: 			var(--cl-yellow-900);
    font-weight: 	600;
}
span.rm-page-ref[data-tag="I"]:after {
    content: 		':';
}```
                - #N → Note to resurface
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
            - Info::
            - Import Instructions::
            - Code::
                - {{[[TODO]]}} Pull in templates
        - Task Management
            - Add
    - Importing Dashboards
        - 
    - Building on the Primitives
    - Clean Up
        - {{[[TODO]]}} Delete any start up templates
