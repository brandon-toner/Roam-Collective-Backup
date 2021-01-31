- #Announcements
    - ## Please document any changes to the CSS under a `#[[Change Log]]` tag within your [[DNP Section]]
- Related:: [[roam/js]]
- Table of Contents::
    - [Tag Styling](((yAzEsiUsx))) ((This needs to be tidied up significantly... ((r1E6gBj56))))
        - [Collections Tags](((JNVnlLDxv))) 
        - [Notifications & Mentions](((01X6uO5N8)))
    - [Block Reference Styling](((xcLgPdvs0)))
    - [Nested Links](((y9rumn-yn)))
- Contents::
    - add `?disablejs=true&disablecss=true` to the end of your roam graph URL, to load without CSS or JS
    - Tips:: Filter by #Status/Enabled in roam/css to view active code. ((This is reliant on updating the tags as things are switched on/off; so may be unreliable))
    - Roam Full Site Themes #Status/Disabled
        - Main CSS (modified [[Leyendecker]])
            - Core
                - ```ruby
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
}

.rm-page-ref-namespace-color {
  color: #2179F3 !important
}

.rm-query {
    border: 0.5px solid #e4e9ec;
    border-radius: 5px;
    
}

.rm-query .rm-query-title {
    background-color: #f7f8f8;
    padding: 0.8em;
    color: #d1dbe2;
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

#block-input {
    background: white;
}

.roam-body #block-input > span > div {
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

#right-sidebar > div {
    background-color: #f7f8fa;
    border-left: 1px solid #e9ebef;
}
.controls .simple-bullet-outer .simple-bullet-inner {
    background-color: #e5e9f2;
}
.block-border-left {
    border-left: 1px solid #f3f6f7;
}
.kanban-board {
    background-color: #fff;
}
.kanban-card {
    background-color: white;
    margin: 8px;
    box-shadow: 0px 1px 2px #9eb3c0a8;
    padding: 10px;
    border-radius: 2px;
    line-height: 1.3em;
}
.kanban-title {
    text-align: center;
    font-weight: 600;
    font-size: 1.1em;
    opacity: 80%;
    color: #485f6f;
    padding-top: 8px;
    border-bottom: 1px solid #c5d1d8;
}
.kanban-column {
    background-color: #e7eff3;
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
    background: #ff913c;
    margin-right: 8px;
}*/

.rm-block-ref {
    border-bottom: none;
    font-size: 1em;
    color: #515e70;
}

.rm-block-ref:hover {
    background: none;
    cursor: pointer;
}
.checkmark {
    background: #fff;
}
.check-container input:checked ~ .checkmark {
    background: #2179F3;
}
.check-container input:checked ~ .checkmark:after {
    border-color: #fff;
}
.rm-reference-item {
    margin-top: 8px;
    border-radius: 6px;
    border: 1px solid #e4e9ee;
    margin-right: 8px;
    flex: 1 1 100%;
    word-break: break-word;
    background-color: #f7f9fb;
    padding: 8px;
}

.rm-level2 {
    font-size: 1.5em;
}
.rm-level3 {
    color: #939aae;
    font-weight: 400;
    font-size: 1.3em;
}
.rm-page-ref {
    color: #4C616A;
}
.rm-page-ref-link-color {
    color: #2179F3;
    font-weight: 600;
}
a {
    color: #2179F3;
}
.intercom-app,
.intercom-launcher-frame,
#intercom-container {
    display: none !important;
}

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
}
#buffer.tall {
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
    background: #fff !important;
    color: #ff4747 !important;
    padding: 4px 14px;
    line-height: 2em;
    font-weight: 600;
    border-radius: 2em;
    border: 1px solid #ff474770;
}

.rm-pomodoro {
    background: #ff6956 !important;
    color: #fff !important;
    padding: 4px 14px;
    line-height: 2em;
    font-weight: 600;
    border-radius: 2em;
    border: 1px solid #ed5845;
}

.rm-pomodoro::first-letter {
  margin-right: 8px;
}```
    - Styling Elements
        1. Tag Styling #Status/Enabled #Highlights #tags
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
                - `#Ideas
                    - ```css
span.rm-page-ref[data-tag="Ideas"] {
    background: #9E9E9E;
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
                - `#[[Open Questions]]
                    - ```css
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
                - `#[[Context Questions]]
                    - ```css
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
    background: #9E9E9E;
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
                - `#Comments
                    - ```css
span.rm-page-ref[data-tag="Comments"] {
    background: #9C27B0;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Comments"]:before {
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
                - `#[[Daily Writing Prompts]]
                    - ```css
span.rm-page-ref[data-tag="Daily Writing Prompts"] {
    background: #4CAF50;
    color: #fff;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

span.rm-page-ref[data-tag="Daily Writing Prompts"]:before {
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
    background: #B1D7B1;
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
        2. Functional CSS
            - Headings & font #Status/Enabled
                - ```css
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
}

.rm-page-ref-link-color {
    color: #2179F3;
    font-weight: 400;
}
a {
    color: #2179F3;
}```
            - Fix sidebar editing height issue #Status/Enabled
                - ```css
/* When editing page title in sidebar this prevents it from having weird height issues */
#right-sidebar .rm-title-textarea {
    width: 95%;
}```
            - Link Symbol #Status/Enabled
                - ```css
.rm-alias-external:before {
    content: '🔗'
}```
                - 
            - Page Reference Underlines & Nested Links #Status/Enabled
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
.rm-page-ref--namespace{
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
            - Block Reference styling #Status/Enabled
                - ```css
.rm-block-ref > span:before {
  content: '| ';
  font-weight: 700;
  color: #FF9800
}```
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
    color: #000000;
    font-weight: 600;
    font-size: 1.3em;
    padding-top: 8px
}
.rm-page-ref {
    color: #0885ff;
}
.rm-page-ref-link-color {
    color: #0885ff;
    font-weight: 600;
}
.rm-ref-page-view-title {
 	font-weight: 600;
 }

#right-sidebar h1.level2 a {
    color: #000000 !important;  
  	font-weight: 400;
    text-decoration: none;
}

/* the location tag is necessary for the above lines to distinguish from external links */```
            - Buttons & Word Count #Status/Enabled
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
        3. Core User Interface ([[e.g.]], Headings)
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
  font-family: var(--fnt-h1);
  font-size: var(--fnt-size-h1);
  font-weight: var(--fnt-weight-h1);
  font-style: var(--fnt-style-h1);
}

h1.level2,
.rm-level2, 
.rm-heading-level-2 > .rm-block__self .rm-block__input {
  font-family: var(--fnt-h2)!important;
  font-size: var(--fnt-size-h2);
  font-weight: var(--fnt-weight-h2);
  font-style: var(--fnt-style-h2);
}

.rm-level3, 
.rm-heading-level-3 > .rm-block__self .rm-block__input {
  font-family: var(--fnt-h3);
  font-size: var(--fnt-size-h3);
  font-weight: var(--fnt-weight-h3);
  font-style: var(--fnt-style-h3);
}

.roam-body .roam-app h1,
.roam-body .roam-app .roam-main .roam-article .rm-title-display {
  font-family: var(--fnt-page-title)!important;
  font-size: var(--fnt-size-page-title);
  color: var(--fg-h1);
}```
        4. Other Styling #frills
            - Left side-bar #Status/Enabled
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
            - Alias Styling
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
  	color: #000000;
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
    border: 1px #bdbdbd dotted;
}

[data-tag="me"] {
    /* Styles */
    color: #000;
    background-color: #c9e33e;
}

[data-tag="ps"] {
    color: white;
    background-color: #5353ff;
}

[data-tag="kap"] {
    color: white;
    background-color: #ff5f5f;
}

[data-tag="Sini"] {
    color: white;
    background-color: #55993a;
}

[data-tag="Roam-Highlights"] {
    color: #b7b7b7;
    background-color: #ffffb4;
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
#right-sidebar .rm-level2, /* page headings in right sidebar */
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
  color: #333 !important;
}

/*a {
    color: #106ba3; 
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

#right-sidebar .controls .roam-bullet-closed,
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
  border-color: #eee;
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
  border-bottom: 0.5px solid #91a8d2; /* darker -Gary */
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

#roam-sidebar-logo img {
  opacity: 0.4;
}
#roam-sidebar-logo span {
  display: none;
}

/* fade loading astrolabe */

.loading-astrolabe img {
  opacity: 0.2;
}

/* lighter sidebar background */

#right-sidebar {
  background-color: rgba(216, 225, 232, 0.2) !important; 
  /* rgba(216, 225, 232, 0.3) */
  border-left: 1px solid #ddd !important;
}

/* sidebar sections */

#roam-right-sidebar-content > div {
  border-bottom: 1px solid #ddd !important;
  margin: 0 !important;
  padding: 10px 4px 10px 50px;
}

/* sidebar section headings */

#roam-right-sidebar-content > div > div:first-child {
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
  border-bottom: 1px solid #eee;
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
  color: #bbb !important;
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
  color: #ddd !important;
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
  border: 1px solid #eee;
  border-radius: 0.3em;
  font-size: 0.8em;
}

.rm-reference-main button:hover {
  border-color: #ccc;
}

/* referenced item section headings */

.rm-reference-main {
  --border-top: 1px solid #ededed;
}

.flex-h-box {
    padding-top: 0px !important;
}

.rm-reference-main .flex-h-box {
  min-height: 30px;
}

.rm-reference-main strong {
  color: #222;
  font-size: 0.9em;
  --background-color: rgba(216, 225, 232, 0.3);
}

/* remove background from referenced items */

.rm-reference-item {
  padding: 6px 0 0 0;
  margin: 6px 0 0 0;
  border-top: 1px solid #eee;
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
  --background-color: #c2f9fa;
}

/* links */

a.rm-alias.rm-alias-external {
    color: #b33ba9 !important;
}

a {
    color: #b33ba9;  
}

.rm-page-ref-link-color {
    color: #106ba3;
}

.rm-ref-page-view-title a{
    color: #106ba3;
    font-weight: bold;
}


.level2 a{
    color: #106ba3;
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
        #right-sidebar {
            #roam-right-sidebar-content {
                .rm-block-text {
                    max-width: 680px;
                }
            }
        }
```
        - Fix for orange blocks
            - ```css
#find-or-create-input {
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
    - Inbox::
        - {{[[TODO]]}} Add #Suggestions to [[roam/css]]
    - Comments::
