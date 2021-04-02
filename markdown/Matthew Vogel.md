- Tags:: #People #Members
    - About me::
        - Twitter:: [@todayIwasbetter](https://twitter.com/todayIwasbetter)
        - Website:: [matt.roam.garden](https://matt.roam.garden) 
__Not nice yet because I can't stop tweaking it long enough to actually get it together__
        - Location:: [[Brooklyn]] [[New York City]] [[United States]]
            - People near me!
                - {{[[query]]: {and:[[Location]] {or:[[Brooklyn]] [[Manhattan]] [[New York]] [[New York City]]} {not:[[query]]}}}}
                - tests
        - Time Zone:: EST [UTC−05:00]
        - Work:: [[Architect]] [[Designer]]
        - How to contact me:: Either twitter or the [[Roam Slack]] works 
        - Interests::[[cooking]] [[architecture]] [[design]] [[metacognition]] comedic [[improvisation]] 
        - **Things I have helped design or develop:**
            - [Journey to the Center of Hawkthorne](http://projecthawkthorne.com/)
            - Spotify's NYC Headquarters
    - {{or:😴Offline | 🟠Away | 🟡On & Off | 🟢Online}}
    - Queries::
        - [[notifications]]
            - {{[[query]]: {and:[[@[[Matthew Vogel]]]] {or:[[cc:[[Matthew Vogel]]]]} {not:[[query]]}}}}
        - Misc useful #datalog #queries
            - [[query]] for all projects
                - :q [:find ?project
	:where 
    	[?e :node/title ?project]
		[(re-matches #"(?i)\b.*(Projects/).*" ?project)]	  
	]
            - Possible to generate a report of "pages authored by graph members"
                - ```javascript
:q [:find ?n 
    :where 
    	[?note :node/title ?n]
		[?bb :block/page ?note] 
		[?bb :block/refs ?p]
		[?bb :block/refs ?c]
		[?c :node/title "Author"]
		[?b :block/page ?p]
		[?b :block/refs ?t]
		[?b :block/refs ?tag]
		[?t :node/title "Members"]
		[?tag :node/title "Tags"]]
```
            - Block with `#tag1` & `#tag2` in contents
                - ```javascript
:q [:find ?blkid ?string
   :where
    [?e :block/uid ?blkid]
   	[?e :block/string ?string]
	[(clojure.string/includes? ?string "#tag1")]
	[(clojure.string/includes? ?string "#tag2")]]```
                    - :q [:find ?blkid ?string
   :where
    [?e :block/uid ?blkid]
   	[?e :block/string ?string]
	[(clojure.string/includes? ?string "#tag1")]
	[(clojure.string/includes? ?string "#tag2")]]
            - [[datalog]] experimentation
                - projects
                    - ```javascript
:q [:find ?project
	:where 
    	[?e :node/title ?project]
		[(re-matches #"(?i)\b.*(Projects/).*" ?project)]	  
	]```
                - attributes
                    - ```javascript
:q [:find ?Namespace ?Attribute
 :where [_ ?Attribute]
[(namespace ?Attribute) ?Namespace]]```
                        - :q [:find ?Namespace ?Attribute
 :where [_ ?Attribute]
[(namespace ?Attribute) ?Namespace]]
                    - ```javascript
:q [:find ?uid
:where
    [?u :user/uid ?uid]
	[?u :user/email "charles.sims.farr@gmail.com"]
   ]```
                        - :q [:find ?uid
:where
    [?u :user/uid ?uid]
	[?u :user/email "charles.sims.farr@gmail.com"]
   ]
                        - "7OcEz5V5OZMBpzWC3Swh4jecQF32"
                - Blocks by user from today
                    - ```javascript
:q [:find ?blkid ?user
   	:where
   	[?b :block/page ?p]
	[?b	:create/user ?u]
	[?u :user/display-name ?user]
	[?p :node/title "February 5th, 2021"]
	[?b	:block/uid ?blkid]
   ]```
                        - :q [:find ?blkid ?user
   	:where
   	[?b :block/page ?p]
	[?b	:create/user ?u]
	[?u :user/display-name ?user]
	[?p :node/title "February 5th, 2021"]
	[?b	:block/uid ?blkid]
   ]
                - Contents of `((3gDduJgIk))` #Scratchpad
                    - ```javascript
:q [:find ?contents ?children
   	:where
   	[?b :block/uid "3gDduJgIk"]
	[?b :block/string ?contents]
	[?b :block/children ?children]]```
                        - :q [:find ?contents ?children
   	:where
   	[?b :block/uid "3gDduJgIk"]
	[?b :block/string ?contents]
	[?b :block/children ?children]]
                    - Block with `eid` = 13163, i.e., `((m4CjJq8zU))`
                        - Feedback: [[Quick Start Guide]]
                        - :q [:find ?attr ?contents
:where
[13163 ?attr ?contents]]
                    - Block with `#tag1` & `#tag2` in contents
                        - ```javascript
:q [:find ?blkid ?string
   :where
    [?e :block/uid ?blkid]
   	[?e :block/string ?string]
	[(clojure.string/includes? ?string "#tag1")]
	[(clojure.string/includes? ?string "#tag2")]]```
                            - :q [:find ?blkid ?string
   :where
    [?e :block/uid ?blkid]
   	[?e :block/string ?string]
	[(clojure.string/includes? ?string "#tag1")]
	[(clojure.string/includes? ?string "#tag2")]]
                - Ancestor Rule
                    - [Source](https://www.putyourleftfoot.in/introduction-to-the-roam-alpha-api)
                    - ```javascript
let ancestorrule='[ [ (ancestor ?b ?a) [?a :block/children ?b] ] [ (ancestor ?b ?a) [?parent :block/children ?b ] (ancestor ?parent ?a) ] ] ]';```
                    - ```javascript
let ancestorrule='[ 
                   [ (ancestor ?b ?a) 
                        [?a :block/children ?b] ] 
                   [ (ancestor ?b ?a) 
                        [?parent :block/children ?b ] 
                        (ancestor ?parent ?a) ] ] ]';```
                    - Trying to parse out exactly how this works...
                        - Create a rule
                            - First vector `(ancestors ?b ?a)` is the head of the rule, with the first symbol "ancestors" being the name
                                - `?b` and `?a` + the following vectors are the body of the rule
                            - The logic of lines 2 & 3 is as follows
                                - Find the eid of a block where `?b` is a children of `?a` **OR** find the eid (`?b`) of the children of `?a`
                            - The logic of lines 4, 5, & 6 is as follows
                                - `?b` is a child of `?parent`
                                - `?parent` is a child of `?a`
                                - Therefore, `?b` is some descendent of `?a`
                                - If you pass in the `?a`, the rule will return all of the children, recursively
                                    - Passes `?a` as the parent recursively until it is at the bottom of the tree
                                    - Rolls up, returning `?b` as all of the child nod
                                - **Note:** I am trying to understand this so don't take the above as fact if you're looking at it... Grasping for straws a bit...
                        - :q [ :find
                  [ (ancestor ?b ?a) 
                        [?a :block/children ?b] ] 
                   [ (ancestor ?b ?a) 
                        [?parent :block/children ?b ] 
                        (ancestor ?parent ?a) ] ] ]
                - Blocks by Author (V1)
                    - ```javascript
[ :find ?author (count ?refs)
	:with ?
    :in $ ?myid %
    :where 
    	[?e :node/title ?myid] 
    	[?b :block/refs ?refs] 
        [?b :create/user ?user]
        [?user :user/display-name ?author]
        (ancestor ?b ?e)]


/*', "February 5th, 2021", ancestorrule */```
                        - :q [:find ?author (count ?refs)
    :where
    [?e :node/title "February 5th, 2021"]
    [?b :block/refs ?refs]
    [?b :create/user ?user]
    [?user :user/display-name ?author]
    [
      [ (ancestor ?b ?a) 
         [?a :block/children ?b] ]
      (ancestor ?b ?a) 
       	[?parent :block/children ?b ] 
       (ancestor ?parent ?a) ]
]
                    - ```javascript
window.roamAlphaAPI.q('[ :find ?author (count ?refs) :with ?e :in $ ?myid % :where [?e :node/title ?myid] [?b :block/refs ?refs] [?b :create/user ?user] [?user :user/display-name ?author] (ancestor ?b ?e)]', "February 5th, 2021", ancestorrule);```
                - Blocks by Author
                    - ```javascript
let query = `[
  :find ?page_title:name ?page_title:uid
  :in $ ?start_of_day %
  :where
  [?page :node/title ?page_title:name]
  [?page :block/uid ?page_title:uid]
  (ancestor ?block ?page)
  [?block :edit/time ?time]
  [(> ?time ?start_of_day)]
]`;```
                    - ```javascript
let rule = `[[ (ancestor ?b ?a) 
             [?a :block/children ?b]] 
             [ (ancestor ?b ?a) 
             [?parent :block/children ?b] 
             (ancestor ?parent ?a)]] 
		    ]`;

let query = `[
	:find ?author (count ?block) (count ?page)
    :in $ ?start_of_day %
    :where 
        [?block :create/user ?user]
        [?user :user/display-name ?author]
  		[?block :create/time ?time]
  		[(> ?time ?start_of_day)]]`

let results = window.roamAlphaAPI.q(query,new Date().setHours(0, 0, 0, 0),rule);

return [query, results];```
                        - {{CLICK TO RUN ADVANCED-QUERY:42SmartBlock:Datomic advanced-query:42RemoveButton=false}}     
                            - :hiccup [:div "Click here to edit block..." [:br][:div {:class "scroller dont-focus-block"}  [:table [:tbody [:tr [:td {:class "head"} "author"][:td {:class "head"} "block"][:td {:class "head"} "page"]][:tr {:class "odd"}[:td {:class "val"}"Charles Farr"][:td {:class "val"}"5"][:td {:class "val"}"5"]]]]]]
                            - :hiccup [:div "Click here to edit block..." [:br][:div {:class "scroller dont-focus-block"}  [:table [:tbody [:tr [:td {:class "head"} "author"][:td {:class "head"} "block"]][:tr {:class "odd"}[:td {:class "val"}"Charles Farr"][:td {:class "val"}"100"]][:tr {:class "even"}[:td {:class "val"}"Brandon Toner"][:td {:class "val"}"10"]][:tr {:class "odd"}[:td {:class "val"}"Peter Rosso"][:td {:class "val"}"40"]][:tr {:class "even"}[:td {:class "val"}"Keifon Lee"][:td {:class "val"}"5"]][:tr {:class "odd"}[:td {:class "val"}"Matt Vogel"][:td {:class "val"}"9"]]]]]]
        - Total Blocks by author
            - ```javascript

let rule = `[[ (ancestor ?b ?a) 
             [?a :block/children ?b]] 
             [ (ancestor ?b ?a) 
             [?parent :block/children ?b] 
             (ancestor ?parent ?a)]] 
		    ]`;

let query = `[
	:find ?author (count ?block)
    :where 
        [?block :create/user ?user]
        [?user :user/display-name ?author]
  		]`

let results = window.roamAlphaAPI.q(query);
results.sort((a, b) => a[1] - b[1]).reverse()
//console.log(sorted)
return [query, results];```
                - {{CLICK TO RUN ADVANCED-QUERY:42SmartBlock:Datomic advanced-query:42RemoveButton=false}}                     
                    - :hiccup [:div "Click here to edit block..." [:br][:div {:class "scroller dont-focus-block"}  [:table [:tbody [:tr [:td {:class "head"} "author"][:td {:class "head"} "block"]][:tr {:class "odd"}[:td {:class "val"}"Brandon Toner"][:td {:class "val"}"4818"]][:tr {:class "even"}[:td {:class "val"}"Charles Farr"][:td {:class "val"}"1743"]][:tr {:class "odd"}[:td {:class "val"}"Keifon Lee"][:td {:class "val"}"351"]][:tr {:class "even"}[:td {:class "val"}"Peter Rosso"][:td {:class "val"}"304"]][:tr {:class "odd"}[:td {:class "val"}"Dhrumil Shah"][:td {:class "val"}"259"]][:tr {:class "even"}[:td {:class "val"}"Matt Vogel"][:td {:class "val"}"256"]][:tr {:class "odd"}[:td {:class "val"}"Mark Robertson"][:td {:class "val"}"92"]][:tr {:class "even"}[:td {:class "val"}"Kyle Stratis"][:td {:class "val"}"46"]][:tr {:class "odd"}[:td {:class "val"}"Eneko Uruñuela"][:td {:class "val"}"40"]][:tr {:class "even"}[:td {:class "val"}"Maggie Delano"][:td {:class "val"}"39"]][:tr {:class "odd"}[:td {:class "val"}"Lindsey Johnston"][:td {:class "val"}"39"]][:tr {:class "even"}[:td {:class "val"}"Michael Shulman"][:td {:class "val"}"38"]][:tr {:class "odd"}[:td {:class "val"}"Beau Haan"][:td {:class "val"}"31"]][:tr {:class "even"}[:td {:class "val"}"Winston"][:td {:class "val"}"20"]][:tr {:class "odd"}[:td {:class "val"}"Alysson M.Costa"][:td {:class "val"}"16"]][:tr {:class "even"}[:td {:class "val"}"Adam Bartley"][:td {:class "val"}"15"]][:tr {:class "odd"}[:td {:class "val"}"Matt Brockwell"][:td {:class "val"}"13"]][:tr {:class "even"}[:td {:class "val"}"Zsolt Viczián"][:td {:class "val"}"12"]][:tr {:class "odd"}[:td {:class "val"}"Wielfried Zouantcha"][:td {:class "val"}"8"]][:tr {:class "even"}[:td {:class "val"}"Tyler Wince"][:td {:class "val"}"7"]][:tr {:class "odd"}[:td {:class "val"}"Chris Kunicki"][:td {:class "val"}"3"]][:tr {:class "even"}[:td {:class "val"}"Mellisa Waltzer"][:td {:class "val"}"2"]][:tr {:class "odd"}[:td {:class "val"}"Palash Karia"][:td {:class "val"}"1"]][:tr {:class "even"}[:td {:class "val"}"Deepu Asok"][:td {:class "val"}"1"]][:tr {:class "odd"}[:td {:class "val"}"Steve Brophy"][:td {:class "val"}"1"]]]]]]
        - My Notes
            - {{[[query]]: {and:[[Matthew Vogel]] [[mtv]] }}}
        - People near me!
            - {{[[query]]: {and:[[Location]] {or:[[Brooklyn]] [[Manhattan]] [[New York]] [[New York City]]} {not:[[query]]}}}}
            - tests
        - tests
            - ```javascript
my db id - 1632
my uid   - "rTvmoxu9FGSWal8SbCZiywCL2Nm1"
:q [:find (pull ?e [[:block/string]
                    [:block/uid]
                    [:edit/time]
                    [:edit/seen-by]]) 
    :where 
    [?f :node/title "Quote"]  
     [?e :block/refs ?f]
    ]


:q [:find (pull ?f [[:block/string]
                    [:block/uid]
                    [:edit/time]
                    [:edit/seen-by]]) 
    :where 
    [?f :block/uid "a8H7Z1PC5"]  
    ]


:q [:find ?members ?uid
 	:where 
    	[?b :user/display-name ?members]
		[?b :user/uid ?uid]
		[?b :db/id] ?id]]

:q [:find (pull ?user [
                    [:user/display-name]
                    ]) 
    :where 
      [?f :block/uid "a8H7Z1PC5"]  
      [?f :edit/user ?user]]

      
      
queryText = `[:find (pull ?e [[:block/string][:block/uid]])
     		            :in $ ?pagetitle
     		            :where
     		                [?f :node/title ?pagetitle]
     		                [?e :block/refs ?f]]`;

          result = window.roamAlphaAPI.q(queryText, "Quotes");
          console.log(result);
```
            - misc queries
                - :q [:find (pull ?user [:user/display-name]) .
    :where 
      [?f :block/uid "a8H7Z1PC5"]  
      [?f :edit/user ?user]]
                - :q [:find ?members 
 	:where 
    	[?b :graph/settings ?members]
		]
                - :q [:find ?members ?uid ?email 
 	:where 
    	[?b :user/display-name ?members]
		[?b :user/uid ?uid]
		[?b :user/email ?email]]
            - [noti queries](((4P2V21RJ3)))
                - Seems like it's missing a step where [[literature notes]] inform/strengthen [["N"-notes]] or would that happen at the [[creative projects]] phase?
                - ```clojure
let query = `[
	:find (pull ?block [{:block/_refs ...}
                        :block/string
                        :block/uid
                        :edit/seen-by
                        :edit/user
                        :edit/time])
    :in $ ?user    
    :where
        [?block :create/user ?user]
        [(missing? $ ?block :node/title)]
        (not [(missing? $ ?block :block/_refs)])

        ]`

let results = window.roamAlphaAPI.q(query,1632);

console.log(results);```
        - noti test
            - [stable Roam42](http://roam42.com/)
                - {{[[roam/js]]}}
                    - ```javascript

// DISABLE FEATURES 
// Remove two forward slashes from in front of name 
// of feature to DISABLE it 
// Everything is enabled by default 
window.disabledFeatures = [ 
  // 'quickReference', 
    // 'turnDown', 
    // 'dateProcessing', 
    // 'lookupUI', 
     'livePreview', 
     'dailyNote', 
    // 'templatePoc', 
    // 'jumpToDate', 
    // 'jumpNav', 
];


var s = document.createElement('script');
	s.type = "text/javascript";
  	s.src =  "https://roam42.glitch.me/main.js";
  	s.async = true;
document.body.appendChild(s);
```
                - {{[[roam/js]]}}
                    - ```javascript

var s = document.createElement('script');
	s.type = "text/javascript";
  	s.src =  "https://roam42.glitch.me/main.js";
  	s.async = true;
document.body.appendChild(s);
```
                - Settings
                    - #42Setting DailyNotePopup off
                    - #42Setting LivePreview off
                - Shortcuts
                    - Natural language date processing -`ALT+SHIFT+D`
            - remove icon flex
                - {{[[roam/js]]}}
                    - ```javascript

var elem = document.getElementById("notification-center-flex");
  elem.parentNode.removeChild(elem);
```
            - remove script
                - {{[[roam/js]]}}
                    - ```javascript

var elem = document.getElementById("roamnotifications");
  elem.parentNode.removeChild(elem);
var elem = document.getElementById("roamnotificationscss");
  elem.parentNode.removeChild(elem);

var elem = document.getElementById("notification-center-button");
  elem.parentNode.removeChild(elem);
```
            - [remote reload](https://github.com/austinbirch/roam-cljs-example)
                - {{[[roam/js]]}}
                    - ```javascript
var s = document.createElement("script");
s.src = "http://127.0.0.1:8081/internal_notifications_masonry.js";
s.id = "roamnotifications";
s.type = "text/javascript";
document.getElementsByTagName("head")[0].appendChild(s);

var ncss = document.createElement("link");
ncss.rel = "stylesheet"
ncss.href = "http://127.0.0.1:8081/notification-center.css";
ncss.id = "roamnotificationscss";
ncss.type = "text/css";
document.getElementsByTagName("head")[0].appendChild(ncss);
```
    - SmartBlocks::#not-populated
    - Bookmarks::
        - [[Evergreens/alert fatigue]]
            - Starter Pack
                - Shortcuts
                    - [[Welcome]]
                    - [[Quick Start Guide]]
                    - [[Conventions]]
                    - [[About Roam Collective]]
                    - [[Directory]]
                    - [[FAQ]]
                - [[Graph/Templates]]
                - [[roam/templates]]
                - [[DNP Modules]]
                - [[Prompts]]
                - [[Announcements]]
                - [[Collections]]
                - [[Conventions]]
            - #Conversation 
            - notifications
                - {{[[mentions]]: [[notification]]}}
            - Expanding features for communication within the graph (in-graph chat, an expanded notification system)
                - A notification system — identifying when you as a user are mentioned within the graph
                - In-graph chat — implemented as an additional sidebar; would allow for slack style chatting, memorialized within a single location within the graph, including native roam features (page and block referencing)
