- **[Tags](<Tags.md>):** [People](<People.md>) [Members](<Members.md>)
    - **[About me](<About me.md>):**
        - **[Twitter](<Twitter.md>):** [@todayIwasbetter](https://twitter.com/todayIwasbetter)
        - **[Website](<Website.md>):** [matt.roam.garden](https://matt.roam.garden) 
__Not nice yet because I can't stop tweaking it long enough to actually get it together__
        - **[Location](<Location.md>):** [Brooklyn](<Brooklyn.md>) [New York City](<New York City.md>) [United States](<United States.md>)
            - {{[embed](<embed.md>): ((((DAqr_IueJ))))}}
        - **[Time Zone](<Time Zone.md>):** EST [UTC−05:00]
        - **[Work](<Work.md>):** [Architect](<Architect.md>) [Designer](<Designer.md>)
        - **[How to contact me](<How to contact me.md>):** Either twitter or the [Roam Slack](<Roam Slack.md>) works 
        - **[Interests](<Interests.md>):**[cooking](<cooking.md>) [architecture](<architecture.md>) [design](<design.md>) [metacognition](<metacognition.md>) comedic [improvisation](<improvisation.md>) 
        - **Things I have helped design or develop:**
            - [Journey to the Center of Hawkthorne](http://projecthawkthorne.com/)
            - Spotify's NYC Headquarters
    - {{or:😴Offline | 🟠Away | 🟡On & Off | 🟢Online}}
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
            - {{[embed](<embed.md>): ((((5FP90Mw7R))))}}
            - {{[embed](<embed.md>): ((((ocuebxkv-))))}}
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
            - {{[query](<query.md>): {and:[Matthew Vogel](<Matthew Vogel.md>) [mtv](<mtv.md>) }}}
        - People near me!
            - {{[query](<query.md>): {and:[Location](<Location.md>) {or:[Brooklyn](<Brooklyn.md>) [Manhattan](<Manhattan.md>) [New York](<New York.md>) [New York City](<New York City.md>)} {not:[query](<query.md>)}}}}
    - **[SmartBlocks](<SmartBlocks.md>):**[not-populated](<not-populated.md>)
    - **[Bookmarks](<Bookmarks.md>):**
        - [Evergreens/alert fatigue](<Evergreens/alert fatigue.md>)
            - Starter Pack
                - Shortcuts
                    - [Welcome](<Welcome.md>)
                    - [Quick Start Guide](<Quick Start Guide.md>)
                    - [Conventions](<Conventions.md>)
                    - [About Roam Collective](<About Roam Collective.md>)
                    - [Directory](<Directory.md>)
                    - [FAQ](<FAQ.md>)
                - [Graph/Templates](<Graph/Templates.md>)
                - [roam/templates](<roam/templates.md>)
                - [DNP Modules](<DNP Modules.md>)
                - [Prompts](<Prompts.md>)
                - [Announcements](<Announcements.md>)
                - [Collections](<Collections.md>)
                - [Conventions](<Conventions.md>)

# Backlinks
## [February 10th, 2021](<February 10th, 2021.md>)
- [Matthew Vogel](<Matthew Vogel.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

## [February 1st, 2021](<February 1st, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

## [February 4th, 2021](<February 4th, 2021.md>)
What does [Everyone](<Everyone.md>) think are the most important workflows/conventions to touch on? [*]([Matthew Vogel](<Matthew Vogel.md>))

- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)[

## [February 5th, 2021](<February 5th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

## [February 6th, 2021](<February 6th, 2021.md>)
- in an [Interintellect](<Interintellect.md>) salon today, [Matthew Vogel](<Matthew Vogel.md>)

## [February 7th, 2021](<February 7th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Matthew Vogel](<Matthew Vogel.md>)

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

