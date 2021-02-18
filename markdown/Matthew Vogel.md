- Tags:: #People #Members
    - About me::
        - Twitter:: [@todayIwasbetter](https://twitter.com/todayIwasbetter)
        - Website:: [matt.roam.garden](https://matt.roam.garden) 
__Not nice yet because I can't stop tweaking it long enough to actually get it together__
        - Location:: [[Brooklyn]] [[New York City]] [[United States]]
            - {{[[embed]]: ((((DAqr_IueJ))))}}
        - Time Zone:: EST [UTC−05:00]
        - Work:: [[Architect]] [[Designer]]
        - How to contact me:: Either twitter or the [[Roam Slack]] works 
        - Interests::[[cooking]] [[architecture]] [[design]] [[metacognition]] comedic [[improvisation]] 
        - **Things I have helped design or develop:**
            - [Journey to the Center of Hawkthorne](http://projecthawkthorne.com/)
            - Spotify's NYC Headquarters
    - Queries::
        - [[notifications]]
            - {{[[query]]: {and:[[@[[Matthew Vogel]]]] {or:[[cc:[[Matthew Vogel]]]]} {not:[[query]]}}}}
        - Misc useful #datalog #queries
            - {{[[embed]]: ((((6zu7U0y7r))))}}
            - "Possible to generate a report of "pages authored by graph members""
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
            - {{[[embed]]: ((((5FP90Mw7R))))}}
            - {{[[embed]]: ((((ocuebxkv-))))}}
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
    - SmartBlocks::#not-populated
    - Bookmarks::
        - [[Evergreens/alert fatigue]]
