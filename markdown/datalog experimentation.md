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
    - Contents of `((3gDduJgIk))` "#Scratchpad"
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
            - "Feedback: [[Quick Start Guide]]"
            - :q [:find ?attr ?contents
:where
[13163 ?attr ?contents]]
        - Block with `#tag1` & `#tag2` in contents
            - ```javascript
:q [:find ?blkid
   :where
    [?e :block/uid ?blkid]
   [?e :block/string ?string]
	[(.contains ^String ?string "#tag1")]]```
                - Does not work at current...
