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
        - My Notes
            - {{[[query]]: {and:[[Matthew Vogel]] [[mtv]] }}}
        - People near me!
            - {{[[query]]: {and: [[Location]] {or: [[Brooklyn]] [[Manhattan]] [[New York]] [[New York City]] }}}}
    - SmartBlocks::#not_populated
    - Bookmarks::
        - [[[[E:]] alert fatigue]]
    - Daily Page Note
        - ;#[[My Daily Notes]] [[Matthew Vogel]] {{word-count}} [*]([[bnt]])   {{or:🟢Online | 😴 offline, back tomorrow | 🟠Away}}
            - #[[Scratchpad]] #not_populated
            - #[[GTD Zone]] #not_populated
            - #[[Change Log]] #not_populated
            - #Promptstorming #not_populated
            - #[[The Zettelkasten]] #not_populated
            - #Conversation #not_populated
                - [[Prompts]]
            - #Feedback  #not_populated
        - ---
