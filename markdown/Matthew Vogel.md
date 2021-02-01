- Tags:: #People #Members
    - About me::
        - Twitter:: [@todayIwasbetter](https://twitter.com/todayIwasbetter)
        - Website:: Not yet because I can't stop tweaking it long enough to actually get it up
        - Location:: [[Brooklyn]] [[New York City]] [[United States]]
        - Time Zone:: EST [UTC−05:00]
        - Work:: [[Architect]] [[Designer]]
        - How to contact me:: Either twitter or the [[Roam Slack]] works 
        - Interests::[[cooking]] [[architecture]] [[design]] [[metacognition]] comedic [[improvisation]] 
        - Queries::
            - [[notifications]]
                - {{[[query]]: {and: {or: {and: [[@]] [[Matthew Vogel]]} [[@[[Matthew Vogel]]]]} {not: [[query]]}} }}
                - {{[[query]]: {and: [[@]] [[Matthew Vogel]] {not: [[query]]}}}}
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
            - My Notes
                - {{[[query]]: {and:[[Matthew Vogel]] [[My Daily Notes]] {not:{or: [[@]] [[~]] }}}}}
            - People near me!
                - {{[[query]]: {and: [[Location]] {or: [[Brooklyn]] [[Manhattan]] [[New York]] [[New York City]] }}}}
        - SmartBlocks::#not_populated
