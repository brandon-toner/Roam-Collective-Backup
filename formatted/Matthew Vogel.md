- **[Tags](<Tags.md>):** [People](<People.md>) [Members](<Members.md>)
    - **[About me](<About me.md>):**
        - **[Twitter](<Twitter.md>):** [@todayIwasbetter](https://twitter.com/todayIwasbetter)
        - **[Website](<Website.md>):** Not yet because I can't stop tweaking it long enough to actually get it up
        - **[Location](<Location.md>):** [Brooklyn](<Brooklyn.md>) [New York City](<New York City.md>) [United States](<United States.md>)
        - **[Time Zone](<Time Zone.md>):** EST [UTC−05:00]
        - **[Work](<Work.md>):** [Architect](<Architect.md>) [Designer](<Designer.md>)
        - **[How to contact me](<How to contact me.md>):** Either twitter or the [Roam Slack](<Roam Slack.md>) works 
        - **[Interests](<Interests.md>):**[cooking](<cooking.md>) [architecture](<architecture.md>) [design](<design.md>) [metacognition](<metacognition.md>) comedic [improvisation](<improvisation.md>) 
    - **[Queries](<Queries.md>):**
        - [notifications](<notifications.md>)
            - {{[query](<query.md>): {and:[@[[Matthew Vogel](<@[[Matthew Vogel.md>)]] {or:[cc:[[Matthew Vogel](<cc:[[Matthew Vogel.md>)]]} {not:[query](<query.md>)}}}}
        - Misc useful [datalog](<datalog.md>) [queries](<queries.md>)
            - {{[embed](<embed.md>): ((((6zu7U0y7r))))}}
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
            - {{[query](<query.md>): {and:[Matthew Vogel](<Matthew Vogel.md>) [mtv](<mtv.md>) }}}
        - People near me!
            - {{[query](<query.md>): {and: [Location](<Location.md>) {or: [Brooklyn](<Brooklyn.md>) [Manhattan](<Manhattan.md>) [New York](<New York.md>) [New York City](<New York City.md>) }}}}
    - **[SmartBlocks](<SmartBlocks.md>):**[not_populated](<not_populated.md>)
    - **[Bookmarks](<Bookmarks.md>):**
        - [[[E:](<[[E:.md>) alert fatigue]]

# Backlinks
## [Directory](<Directory.md>)
- [Matthew Vogel](<Matthew Vogel.md>)

## [February 1st, 2021](<February 1st, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

## [February 4th, 2021](<February 4th, 2021.md>)
What does [Everyone](<Everyone.md>) think are the most important workflows/conventions to touch on? [*]([Matthew Vogel](<Matthew Vogel.md>))

- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)[

## [January 27th, 2021](<January 27th, 2021.md>)
- Adjusted not-populated to not_populated based on [Matthew Vogel](<Matthew Vogel.md>)'

- PS, to send a notification, use the @ symbol rather than ~ to indicated "unread" status. When read, you can replace with a ~ to indicate read. [~](<~.md>) [Matthew Vogel](<Matthew Vogel.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

- "PS, to send a notification, use the @ symbol rather than ~ to indicated "unread" status. When read, you can replace with a ~ to indicate read. [~](<~.md>) [Matthew Vogel](<Matthew Vogel.md>)"

- 11:54 - [Matthew Vogel](<Matthew Vogel.md>)

## [January 28th, 2021](<January 28th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

- A Roaman ([e.g.](<e.g..md>) [Matthew Vogel](<Matthew Vogel.md>))

## [January 29th, 2021](<January 29th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

## [January 31st, 2021](<January 31st, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

## [Matthew Vogel](<Matthew Vogel.md>)
- {{[query](<query.md>): {and:[Matthew Vogel](<Matthew Vogel.md>)

## [Projects/Establish automated graph backups](<Projects/Establish automated graph backups.md>)
- [Matthew Vogel](<Matthew Vogel.md>)

