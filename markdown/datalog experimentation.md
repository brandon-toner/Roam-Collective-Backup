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
