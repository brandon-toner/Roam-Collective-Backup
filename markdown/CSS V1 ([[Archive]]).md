- ## Shortcuts:
    - [Colors](((ClLqIfFSn)))
    - [Tag Styling](((6w_N1hr1k)))
        - [Collections Tags](Page-type Tags) 
        - [Notifications & Mentions](Notifications & Mentions)
    - [Headings](((nL58k_bhI)))
    - [Page References](((kJ_piMpzy)))
    - [Block References](((xcLgPdvs0)))
    - [External Links](((r3wJzzQJP)))
    - [Aliases](((MLfGQ-X-L)))
    - [Nested Links](((y9rumn-yn)))
    - [Queries](((KOuJf-Smr)))
- ## Code:
    - Elements
        - Tags
            - Top-Section Tags
                - #[[Community Notes]] [[Roam Collective]]
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
                - #[[Voting]]
                    - ```css
span.rm-page-ref[data-tag="Voting"] {
    background: #607D8B;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Voting"]:before {
    content: '🗳'
}```
                - #Announcements
                    - ```css
span.rm-page-ref[data-tag="Announcements"] {
    background: 	var(--cl-red-800);
    color: 			var(--cl-white);
    padding: 		2px 5px 2px 5px;
    font-size: 		13px;
    line-height: 	1em;
    font-weight: 	500;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
}

span.rm-page-ref[data-tag="Announcements"]:before {
    content: 		'📢';
  	padding-right: 	2px;
}```
                - #[[Daily Activities]]
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
                - #[[Main Feed]]
                    - ```css
span.rm-page-ref[data-tag="Main Feed"] {
	background: 	var(--cl-blue-700);
    color: 			var(--cl-white);
    padding: 		2px 5px 2px 5px;
    font-size: 		13px;
    line-height: 	1em;
    font-weight: 	500;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
}

span.rm-page-ref[data-tag="Main Feed"]:before {
    content:     	'⭐️';
  	padding-right: 	2px;
}```
                - #[[Graph Change Log]]
                    - ```css
span.rm-page-ref[data-tag="Graph Change Log"] {
	background: 	var(--cl-gray-800);
    color: 			var(--cl-white);
    padding: 		2px 5px 2px 5px;
    font-size: 		13px;
    line-height: 	1em;
    font-weight: 	500;
    border-radius: 	5px 5px 5px 5px;
    position:		relative;
}

span.rm-page-ref[data-tag="Graph Change Log"]:before {
    content:     	'⚙️';
  	padding-right: 	2px;
}```
            - DNP Modules
                - #[[My Daily Notes]] [[Your Name]]
                    - ```html
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
}

span.rm-page-ref[data-tag="My Daily Notes"] + span[data-link-title] > .rm-page-ref::before
{
  content:			"ᐅ";
  color: 			var(--cl-yellow-900);
  padding-right:	5px;
  font-weight:		900;
}
```
                - #Scratchpad
                    - ```html
span.rm-page-ref[data-tag="Scratchpad"] 
{ background: #fff;
  background-size: 100%;
  color: #000;
  padding: 2px 5px 2px 5px;
  font-size: 13px;
  line-height: 1em;
  font-weight: 500;
  border-radius: 5px 5px 5px 5px;
  border-style: solid;
  border-color: var(--cl-gray-800);
  border-width: thin;
  position:relative;
  box-shadow: 0px 1px 3px -1px #000000, 0px -1px 3px  #DFDFDF;
}

span.rm-page-ref[data-tag="Scratchpad"]:before {
    content: 	'✏️';
  	padding-right:	2px;
}```
                - #[[Conversation & Comments]]
                    - ```html
span.rm-page-ref[data-tag="Conversation"] 
{ background: #fff;
  background-size: 100%;
  color: #000;
  padding: 2px 5px 2px 5px;
  font-size: 13px;
  line-height: 1em;
  font-weight: 500;
  border-radius: 5px 5px 5px 5px;
  border-style: solid;
  border-color: var(--cl-gray-700);
  border-width: thin;
  position:relative;
  box-shadow: 0px 1px 3px -1px #000000, 0px -1px 5px  #DFDFDF;
}

span.rm-page-ref[data-tag="Conversation"]:before {
    content: 		'📮';
  	padding-right: 	2px;
}```
                - #[[Change Log]]
                    - ```html
span.rm-page-ref[data-tag="Change Log"] 
{ background: #fff;
  background-size: 100%;
  color: #000;
  padding: 2px 5px 2px 5px;
  font-size: 13px;
  line-height: 1em;
  font-weight: 500;
  border-radius: 5px 5px 5px 5px;
  border-style: solid;
  border-color: var(--cl-gray-800);
  border-width: thin;
  position:relative;
  box-shadow: 0px 1px 3px -1px #000000, 0px -1px 5px  #DFDFDF;
}

span.rm-page-ref[data-tag="Change Log"]:before {
    content: '📢';
  	padding-right: 2px;  
}```
                - #[[Feedback]]
                    - ```html
span.rm-page-ref[data-tag="Feedback"] 
{ background: #fff;
  background-size: 100%;
  color: #000;
  padding: 2px 5px 2px 5px;
  font-size: 13px;
  line-height: 1em;
  font-weight: 500;
  border-radius: 5px 5px 5px 5px;
  border-style: solid;
  border-color: var(--cl-purple-900);
  border-width: thin;
  position:relative;
  box-shadow: 0px 1px 3px -1px #000000, 0px -1px 5px  #DFDFDF;
}

span.rm-page-ref[data-tag="Feedback"]:before {
    content: '💬';
  	padding-right: 2px;  
}```
                - #[[Bookmarks]]
                    - ```html
span.rm-page-ref[data-tag="Bookmarks"] 
{ background: #fff;
  background-size: 100%;
  color: #000;
  padding: 2px 5px 2px 5px;
  font-size: 13px;
  line-height: 1em;
  font-weight: 500;
  border-radius: 5px 5px 5px 5px;
  border-style: solid;
  border-color: var(--cl-gray-700);
  border-width: thin;
  position:relative;
  box-shadow: 0px 1px 3px -1px #000000, 0px -1px 5px  #DFDFDF;
}

span.rm-page-ref[data-tag="Bookmarks"]:before {
    content: '💾';
  	padding-right: 2px;
}```
                - #Todos
                    - ```html
span.rm-page-ref[data-tag="Todos"] 
{ background: #fff;
  background-size: 100%;
  color: #000;
  padding: 2px 5px 2px 5px;
  font-size: 13px;
  line-height: 1em;
  font-weight: 500;
  border-radius: 5px 5px 5px 5px;
  border-style: solid;
  border-color: var(--cl-gray-700);
  border-width: thin;
  position:relative;
  box-shadow: 0px 1px 3px -1px #000000, 0px -1px 5px  #DFDFDF;
}

span.rm-page-ref[data-tag="Todos"]:before {
    content: 		'🎯';
  	padding-right: 	2px;
}```
                - #[[Daily Log]]
                    - ```html
span.rm-page-ref[data-tag="Daily Log"] 
{ background: #fff;
  background-size: 100%;
  color: #000;
  padding: 2px 5px 2px 5px;
  font-size: 13px;
  line-height: 1em;
  font-weight: 500;
  border-radius: 5px 5px 5px 5px;
  border-style: solid;
  border-color: var(--cl-gray-700);
  border-width: thin;
  position:relative;
  box-shadow: 0px 1px 3px -1px #000000, 0px -1px 5px  #DFDFDF;
}

span.rm-page-ref[data-tag="Daily Log"]:before {
    content: '📆'
}```
            - Note & Zettelkasten Tags
                - #[[LN]] 
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
                - #Prop
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
                - #[[Seedlings]]
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
                - #[[Buddings]]
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
                - #[[Project Ideas]]
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
}```
                - #[[Annotations]]
                    - ```css
span.rm-page-ref[data-tag="Annotations"] {
	background: #795548;
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
                            - Example: #Evergreens Prefer note titles with complete phrases to sharpen claims
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
                    - #[[Community Note]] [[Test]]
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
                            - Example: #Evergreens Prefer note titles with complete phrases to sharpen claims
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
                    - #Notion #Test
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
                    - #Syn #Test
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
                    - #Obs 
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
                    - #[[Branching Notes]] [[Test]]
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
                    - #[[Zettel Questions]]
                        ```css
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
}```
                    - #[[Intermediary Notes]]
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
}```
            - Prepositional Linkages
                - #therefore
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
            - Feedback Tags
                - #Feedback
                    - #[[[[Feedback]]: What's working]]
                    - #[[[[Feedback]]: What could be better]]
                    - #[[[[Feedback]]: [[Suggestions]]]]
                    - Code
                        - ```clojure
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
                - #[[Bug Reports]]
                    - ```css
span.rm-page-ref[data-tag="Bug Reports"] {
    color: var(--tag-text-cl);
    font-weight: 450;
}```
                - #[[Roam Enhancement Requests]]
                    - ```css
span.rm-page-ref[data-tag="Roam Enhancement Requests"] {
    color: var(--tag-text-cl);
    font-weight: 450;
}```
            - Processing Tags
                - `#[[Housekeeping]]
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
            - Highlight Tags
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
                - #[[My Wins]]
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
                - #[[Random Review]]
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
            - Journaling Tags
                - `#[[Reflection]]
                    - ```css
span.rm-page-ref[data-tag="Reflection"] {
    background: #607D8B;
    color: #fff;
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
            - Status Tags
                - Examples
                    - #[[Status/Idea]]
                        - ```css
```
                    - #[[Status/Active]]
                        - ```css
```
                    - #Status/On-Hold
                        - ```css
```
                    - #[[Status/Dropped]]
                        - ```css
```
                    - #Status/Enabled
                        - ```css
```
                    - #Status/Inactive
                        - ```css
```
                    - #Status/Submitted
                        - ```css
```
                    - #Status/Completed
                        - ```css
```
                    - #Status/Deactivated
                        - ```css
```
                    - #[[Status/Someday|Maybe]]
                        - ```css
```
                    - #[[Status/Not Completed]]
                        - ```css
```
                - Code
                    - ```css
:root {
  --status-padding: 1px 1px 1px 1px;
}

span.rm-page-ref[data-tag="Status/Sent"] {
    background: #03A9F4;
    color: #fff;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Resolved"] {
    background: #8BC34A;
    color: #fff;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Closed"] {
    background: #000000;
    color: #fff;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Completed"] {
    color: #4CAF50;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Incomplete"] {
    color: #607D8B;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Waiting-For"] {
    color: #795548;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/On-Hold"] {
    color: #6A6A6A;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Dropped"] {
    color: #C30D00;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Active"] {
    color: #2196F3;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Approved"] {
    color: #4CAF50;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Someday|Maybe"] {
    color: #467C96;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Not-Completed, Carried"] {
    color: #FF9800;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Status/Enabled"] {
    color: #4CAF50;
    padding: var(--status-padding);
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}```
            - Miscellaneous
                - `#[[Quick Capture]]
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
                - `#Problems
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
            - Experimental
                - `#Quote (inline block ref)
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
                - [Personas](https://www.rodrigofranco.com/roam-personas-css.html) #Experiments
                    - Examples
                        - #[[P:Self]] Inner Self Talk
                        - #[[P:Loving]] Love thyself
                        - #[[P:Critic]] Hard on yourself
                    - Code
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
            - Archived & Deprecated
                - Depreciated
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
                    - `#Reply-from [[your_name_here]]`
                        - ```html
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
                    - `#[[Posted by]] [[your_name_here]]`
                    - #Help [[your_name_here]]
                        - ```html
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
                    - #@ [[your_name_here]]
                        - ```html
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
                - `#Resolved`
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
                - `#Happenings`
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
                - `#Disabled`
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
                - `#Important`
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
                - `#Urgent`
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
                - `Alert/ tags`
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
                - `#Flag`
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
                - `Flag/ tags`
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
                - `SCC/ tags`
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
                - `#[[Focus Mode (plus)]]`
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
                - `#[[Action Items]]`
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
                - `Evergreen tags` (#Legacy)
                    - ```html
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
        - User Interface
        - Content
        - Miscellaneous
    - Patch Fixes
        - Fix for orange blocks ((Unsure purpose - BT))
            - ```css
#find-or-create-input {
   outline: none!important;
}```
    - Archive
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
