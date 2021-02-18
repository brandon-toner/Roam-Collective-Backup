- **[Tags](<../Tags.md>):** [Collections](<../Collections.md>)
- **[Related](<../Related.md>):** [roam](<../roam.md>)/templates
- **[Table of Contents](<../Table of Contents.md>):**
    - [Global Variables](((bFUOGEPXz)))
    - [Daily Templates](((dho4joU3n)))
    - [Dates](((hnK4dsiz3)))
    - [Productivity](((HjC43lt9e)))
    - [Page Templates](((yURo5cs1L)))
    - [Algorithms of Thought](((xl1VDddLC)))
    - [Randomization](((yEt_7OyoF)))
    - Used as Buttons
        - [Waiting](((P5Ov0rVPM)))
    - [Miscellaneous](((3Oj1R8i4j)))
- **[Contents](<../Contents.md>):**
    - Global Variables
        - [42Setting](<../42Setting.md>) ThisWeek #[Week-07: 02-15-2021](<../Week-07: 02-15-2021.md>)
        - [42Setting](<../42Setting.md>) ThisWkRaw Week-07: 02-15-2021
        - [42Setting](<../42Setting.md>) NextWeek #[Week-08: 02-22-2021](<../Week-08: 02-22-2021.md>)
        - [42Setting](<../42Setting.md>) NextWkRaw Week-08: 02-22-2021
        - [42Setting](<../42Setting.md>) ThisMonth #[February 2021](<../February 2021.md>)
        - [42Setting](<../42Setting.md>) ThisMnthRaw February 2021
        - [42Setting](<../42Setting.md>) NextMonth #[March 2021](<../March 2021.md>)
        - [42Setting](<../42Setting.md>) NextMnthRaw March 2021
    - Daily Templates
        - .rc2DH — Daily Header [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - {{embed: ((FRFW0hQu_))}}
            - ---
            - #[My Daily Notes](<../My Daily Notes.md>) [Roam-Collective](<../Roam-Collective.md>) {{word-count}} [*]([rc](<../rc.md>)) 
                - #[Daily Activities](<../Daily Activities.md>) ((Prompts to expand our knowledge base. If not already selected, choose one or more from the Prompts page.))
                    - "Choose whatever tickles your fancy from the [prompts list]([Prompts](<../Prompts.md>)) ((Don't forget to nest your responses under the Promptstorming tag))"
                - #[The Main Feed](<../The Main Feed.md>) ((A place to showcase graph highlights throughout the day)) [not-populated](<../not-populated.md>) 
                - [Chat](<../Chat.md>) ((A place to propose objects of discussion)) [not-populated](<../not-populated.md>)
                - #[GTD Zone](<../GTD Zone.md>) ((Run the "Daily Review" smartblock)) [not-populated](<../not-populated.md>) 
            - ---
        - .rc1DNP — Daily Notes Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - #[My Daily Notes](<../My Daily Notes.md>) [your_name_here](<../your_name_here.md>) {{word-count}}
                - ^^Replace "your name here" with your page link^^
                - [Scratchpad](<../Scratchpad.md>) ((Use this as scrap paper. A place to jot down you ideas))[not-populated](<../not-populated.md>)
                - [Questions](<../Questions.md>) ((about the graph, or directed towards someone)) [not-populated](<../not-populated.md>)
                - [Conversation](<../Conversation.md>) [not-populated](<../not-populated.md>)
                - [Feedback](<../Feedback.md>) ((share your comments about the experience, click on the feedback tag for more info)) [not-populated](<../not-populated.md>)
                - For descriptions of the other "DNP Modules", visit this page → `[DNP Modules](<../DNP Modules.md>)`
                - ---
    - Dates
        - .rc3TD — Today [42SmartBlock](<../42SmartBlock.md>)
            - <%DATE:today%>
        - .rc3TMRW — Tomorrow [42SmartBlock](<../42SmartBlock.md>)
            - <%DATE:tomorrow%>
        - .rc4WK — This Week [42SmartBlock](<../42SmartBlock.md>)
            - <%42SETTING:ThisWeek%>
        - .rc4MNTH — This Month [42SmartBlock](<../42SmartBlock.md>)
            - <%42SETTING:ThisMonth%>
        - .rc4NW — Next Week [42SmartBlock](<../42SmartBlock.md>)
            - <%42SETTING:NextWeek%>
        - .rc4NM — Next Month [42SmartBlock](<../42SmartBlock.md>)
            - <%42SETTING:NextMonth%>
    - Productivity
        - .rc3GTD — Daily Review GTD [42SmartBlock](<../42SmartBlock.md>)
            - **[Daily Review](<../Daily Review.md>):**
                - **Scheduled for Today:**
                    - <%IFDAYOFWEEK:1,2%> [ ] Update week variables <%DATE:Today%>
                        - {{[embed](<../embed.md>): ((bFUOGEPXz))}}
                    - <%IFDAYOFMONTH:1,2%> [ ] Update month variables <%DATE:Today%>
                        - {{[embed](<../embed.md>): ((bFUOGEPXz))}}
                    - **Page:** <%PAGE%>
{{[embed](<../embed.md>): <%BLOCKMENTIONS:20,TODO,<%DATE:today%>,-DONE%>}}
                - {{Overdue:42SmartBlock:.rc3TODO — TODO Overdue (10, with header)}}
                - {{Flagged:42SmartBlock:.rc4FLG — Flagged}}
                - {{Waiting:42SmartBlock:.rc3WAIT — Waiting}}
                - {{TODO This Week:42SmartBlock:.rc3TODO — TODO This Week}}
                - {{TODO This Month:42SmartBlock:.rc3TODO — TODO This Month}}
            - **Ways you can help:**
                - __Check out the linked references on the Help Wanted tag for more other ways you can contribute.__ Thanks for being here 😄
                - **Results:** <%BLOCKMENTIONS:-1,TODO,Help Wanted,-DONE,-query,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[embed](<../embed.md>): <%BLOCKMENTIONS:20,TODO,Help Wanted,-DONE,-query,-`%>}}
        - .rc4FLG — Flagged [42SmartBlock](<../42SmartBlock.md>)
            - **Flagged:**
                - **Results:** <%BLOCKMENTIONS:-1,Flagged,-query,-DONE,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[embed](<../embed.md>): <%BLOCKMENTIONS:20,Flagged,-query,-DONE,-`%>}}
        - .rc3WAIT — Waiting [42SmartBlock](<../42SmartBlock.md>)
            - **Waiting:**
                - **Results:** <%BLOCKMENTIONS:-1,Waiting,-DONE,-query,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[embed](<../embed.md>): <%BLOCKMENTIONS:20,Waiting,-DONE,-query,-`%>}}
        - .rc3TODO — Scheduled for Today [42SmartBlock](<../42SmartBlock.md>)
            - **Scheduled for Today:**
                - **Page:** <%PAGE%>
{{[embed](<../embed.md>): <%BLOCKMENTIONS:20,TODO,<%DATE:today%>,-DONE%>}}
        - .rc3TODO — TODO Overdue (10, with header) [42SmartBlock](<../42SmartBlock.md>)
            - **Overdue TODOs:**  
                - {{[embed](<../embed.md>): <%TODOOVERDUE:10%>}}
        - .rc3TODO — TODO This Week [42SmartBlock](<../42SmartBlock.md>) 
            - **This Week:** `<%42SETTING:ThisWeek%>`
                - **Results:** <%BLOCKMENTIONS:-1,TODO,<%42SETTING:ThisWkRaw%>,-DONE%> **Max:** 25
                - **Page:** <%PAGE%>
{{[embed](<../embed.md>): <%BLOCKMENTIONS:25,TODO,<%42SETTING:ThisWkRaw%>,-DONE%>}}
        - .rc3TODO — TODO This Month [42SmartBlock](<../42SmartBlock.md>)
            - **This Month:** `<%42SETTING:ThisMonth%>`
                - **Results:** <%BLOCKMENTIONS:-1,TODO,<%42SETTING:ThisMnthRaw%>,-DONE%> **Max:** 25
                - **Page:** <%PAGE%>
{{[embed](<../embed.md>): <%BLOCKMENTIONS:25,TODO,<%42SETTING:ThisMnthRaw%>,-DONE%>}}
        - .rc3TODO — TODO Help Wanted [42SmartBlock](<../42SmartBlock.md>)
            - **Ways you can help:**
                - __Check out the linked references on the Help Wanted tag for more other ways you can contribute.__ Thanks for being here 😄
                - **Results:** <%BLOCKMENTIONS:-1,TODO,Help Wanted,-DONE,-query,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[embed](<../embed.md>): <%BLOCKMENTIONS:20,TODO,Help Wanted,-DONE,-query,-`%>}}
    - Page Templates
        - .rc3PRSNL — Personal Page [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [People](<../People.md>) [Members](<../Members.md>)
                - **[About me](<../About me.md>):**
                    - **[Twitter](<../Twitter.md>):** [not-populated](<../not-populated.md>)
                    - **[Website](<../Website.md>):** [not-populated](<../not-populated.md>) 
                    - **[Location](<../Location.md>):** [not-populated](<../not-populated.md>)
                    - **[Time Zone](<../Time Zone.md>):** [not-populated](<../not-populated.md>)
        - .rc2PRJ — Projects Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Projects](<../Projects.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Related](<../Related.md>):** #[not-populated](<../not-populated.md>)
                - **[People](<../People.md>):** #[not-populated](<../not-populated.md>) [Housekeeping](<../Housekeeping.md>)
                    - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                    - **[Project Lead](<../Project Lead.md>):** [not-populated](<../not-populated.md>)
                    - **[Contributors](<../Contributors.md>):** [not-populated](<../not-populated.md>)
                - **[Areas](<../Areas.md>):** #[not-populated](<../not-populated.md>) [Housekeeping](<../Housekeeping.md>)
                - **[Project Status](<../Project Status.md>):** #[not-populated](<../not-populated.md>) [Housekeeping](<../Housekeeping.md>)
                - **[Due Date](<../Due Date.md>):** #[not-populated](<../not-populated.md>) [Housekeeping](<../Housekeeping.md>)
                - **[Reminders](<../Reminders.md>):** #[not-populated](<../not-populated.md>) 
                - **[Date Completed](<../Date Completed.md>):** #[Status/Not Completed](<../Status/Not Completed.md>)
                - **[Notes](<../Notes.md>):** #[not-populated](<../not-populated.md>)
                - **[Tasks](<../Tasks.md>):** [not-populated](<../not-populated.md>)
        - .rc3REF — Reference Note Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Resources](<../Resources.md>) #[Reference Notes](<../Reference Notes.md>) ((add type of resource... Articles, Books, Videos etc.))
                - **[Author(s)](<../Author(s).md>):** [not-populated](<../not-populated.md>)
                - **[Full Title](<../Full Title.md>):** [not-populated](<../not-populated.md>)
                - **[URL](<../URL.md>):** [not-populated](<../not-populated.md>)
        - .rc3CRT — Creative Project Template [42SmartBlock](<../42SmartBlock.md>) #[roam/templates](<../roam/templates.md>)
            - **[Tags](<../Tags.md>):** [Projects](<../Projects.md>) [Creative](<../Creative.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Resources](<../Resources.md>):** [not-populated](<../not-populated.md>)
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>)
                - **[Outline](<../Outline.md>):** [not-populated](<../not-populated.md>)
                - **[Next Steps](<../Next Steps.md>):** [not-populated](<../not-populated.md>) ((Plans for future elaboration or development))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
        - .rc3SPR — Sprints Template [42SmartBlock](<../42SmartBlock.md>) #[roam/templates](<../roam/templates.md>)
            - **[Tags](<../Tags.md>):** [Sprints](<../Sprints.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Date Range](<../Date Range.md>):** [not-populated](<../not-populated.md>)
                - **[Description](<../Description.md>):** [not-populated](<../not-populated.md>)
                - **[Status](<../Status.md>):** [not-populated](<../not-populated.md>)
                - **[Resources](<../Resources.md>):** [not-populated](<../not-populated.md>)
                - **Outlines:** [not-populated](<../not-populated.md>) ((Replace ex-A with the sprint page name))
                    - **[Query](<../Query.md>):**
                        - {{[query](<../query.md>): {and: [ex-A](<../ex-A.md>) [Outlines](<../Outlines.md>)}}} [minimal](<../minimal.md>)
                - **Questions:** [not-populated](<../not-populated.md>) ((Replace ex-A with the sprint page name))
                    - **[Query](<../Query.md>):**
                        - {{[query](<../query.md>): {and: [ex-A](<../ex-A.md>) {or: [Q](<../Q.md>) [Questions](<../Questions.md>)}}}} [minimal](<../minimal.md>)
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>) ((Replace ex-A with the sprint page name))
                    - **[Query](<../Query.md>):**
                        - {{[query](<../query.md>): {and: [ex-A](<../ex-A.md>) {or: [E:](<../E:.md>) [FN](<../FN.md>) [I](<../I.md>) [Literature Notes](<../Literature Notes.md>)}}}} [minimal](<../minimal.md>)
                - **[Tasks](<../Tasks.md>):** [not-populated](<../not-populated.md>) ((Replace ex-A with the sprint page name))
                    - **[Query](<../Query.md>):** 
                        - {{[query](<../query.md>): {and: [ex-A](<../ex-A.md>) [TODO](<../TODO.md>)}}}
                - **[Work Summary](<../Work Summary.md>):** [not-populated](<../not-populated.md>) ((Include your name, the date, a description of the work, and a link to the work))
        - .rc3EPC — Epics Template [42SmartBlock](<../42SmartBlock.md>) #[roam/templates](<../roam/templates.md>)
            - **[Tags](<../Tags.md>):** [Epics](<../Epics.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Date Range](<../Date Range.md>):** [not-populated](<../not-populated.md>)
                - **[Description](<../Description.md>):** [not-populated](<../not-populated.md>)
                - **[Status](<../Status.md>):** [not-populated](<../not-populated.md>)
                - **[Resources](<../Resources.md>):** [not-populated](<../not-populated.md>)
                - **[Work Summary](<../Work Summary.md>):** [not-populated](<../not-populated.md>) ((Include your name, the date, a description of the work, and a link to the work))
        - .rcEVN — Evergreen Note Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** #[Evergreens](<../Evergreens.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Author](<../Author.md>):** [not-populated](<../not-populated.md>)
                - **[References](<../References.md>):** [not-populated](<../not-populated.md>) ((Supporting FN, LN, EN, or RN would go here))
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>) ((Not a reference, but a related idea, block or page))
                - **[Next Steps](<../Next Steps.md>):** [not-populated](<../not-populated.md>) ((Plans for future elaboration or development))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
        - .rcPVB — Proverb Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Proverbs](<../Proverbs.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Origin](<../Origin.md>):** [not-populated](<../not-populated.md>)
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>) ((Not a reference, but a related idea, block or page))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
        - .rcSDL — Seedlings Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Seedlings](<../Seedlings.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Author](<../Author.md>):** [not-populated](<../not-populated.md>)
                - **[References](<../References.md>):** [not-populated](<../not-populated.md>) ((Supporting FN, LN, EN, or RN would go here))
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>) ((Not a reference, but a related idea, block or page))
                - **[Next Steps](<../Next Steps.md>):** [not-populated](<../not-populated.md>) ((Plans for future elaboration or development))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
        - .rcQST — Questions Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Questions](<../Questions.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.rc3TD — Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Author](<../Author.md>):** [not-populated](<../not-populated.md>)
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>) ((Related notes in the graph — FN, LN, EN, Q, I, etc.))
                - **[Next Steps](<../Next Steps.md>):** [not-populated](<../not-populated.md>) ((Plans for future elaboration or development))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
                - **[Work Summary](<../Work Summary.md>):** [not-populated](<../not-populated.md>) ((Link to work related to this page from elsewhere in the graph — Include name & date if relevant))
    - Algorithms of Thought
        - .rc3CH — Choice AoT [roam](<../roam.md>)/templates
            - [ ] [Choice](<../Choice.md>):  ((((e-lL4buZ1))))
                - **[Options](<../Options.md>):** [not-populated](<../not-populated.md>)
                - **[Status](<../Status.md>):** [not-populated](<../not-populated.md>)
                - **[Decision](<../Decision.md>):** [not-populated](<../not-populated.md>)
                - **[Notes](<../Notes.md>):** [not-populated](<../not-populated.md>)
        - .rc3CH — Choice Options [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - <%INPUT:Letter (e.g. A, B, C)%%A%> -
                - **[Pros](<../Pros.md>):** [not-populated](<../not-populated.md>)
                - **[Cons](<../Cons.md>):** [not-populated](<../not-populated.md>)
    - Randomization 
        - .rc3RFN — Random Fleeting Note (Experimental) [42SmartBlock](<../42SmartBlock.md>) ((Not truly random...))
            - ^^Reminder:^^ __Please delete any block references where you did not add any annotations to prevent "empty references"__
            - **Page:** `<%PAGE%>`
<%BLOCKMENTIONS:<%INPUT:How may would you like to return?%%3%>,Fleeting Notes%>
        - .rc3RFN — Random Fleeting Note (Experimental) (no instructions) [42SmartBlock](<../42SmartBlock.md>) ((Not truly random...))
            - **Page:** `<%PAGE%>`
<%BLOCKMENTIONS:<%INPUT:How may would you like to return?%%3%>,Fleeting Notes%>
        - .rc3RSL — Random Seedling (Experimental) [42SmartBlock](<../42SmartBlock.md>) ((Not truly random...))
            - ^^Reminder:^^ __Please delete any block references where you did not add any annotations to prevent "empty references"__
            - **Page:** `<%PAGE%>`
<%BLOCKMENTIONS:<%INPUT:How may would you like to return?%%3%>,Seedlings%> 
        - .rc3RSL — Random Seedling (no instructions) (Experimental) [42SmartBlock](<../42SmartBlock.md>) ((Not truly random...))
            - **Page:** `<%PAGE%>`
<%BLOCKMENTIONS:<%INPUT:How may would you like to return?%%3%>,Seedlings%> 
        - ,rcREN — Random Evergreen Note (Experimental) [42SmartBlock](<../42SmartBlock.md>)
            - ^^Reminder:^^ __Please delete any block references where you did not add any annotations to prevent "empty references"__ ((The block reference generated is not important, that can be deleted.))
            - <%PAGE%>
((<%BLOCKMENTIONS:1,Evergreen Notes,Tags%>)) 
        - ,rcREN — Random Evergreen Note (no instructions) (Experimental) [42SmartBlock](<../42SmartBlock.md>)
            - <%PAGE%>
((<%BLOCKMENTIONS:1,Evergreen Notes,Tags%>)) 
    - Miscellaneous
        - .rc2CSS — Add to CSS [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - [ ] Add to [roam/css](<../roam/css.md>)
        - ,rcTEN — "in tension with" [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - in [tension]([Tensions](<../Tensions.md>)) with
        - .rc1BRK — Horizontal Rule [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - ---
        - .rcDRP — Dropdown Menu [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - {{or: Option A | Option B | Option C}}
        - .rcBRB — Online/Status [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - {{or:🟢Online | 😴 offline, back tomorrow | 🟠Away}}
        - [42SmartBlock](<../42SmartBlock.md>) .rcNotify — @Everyone Tag
            - {{or: [@[[Everyone](<../@[[Everyone.md>)]] | [@[[Charles Farr](<../@[[Charles Farr.md>)]] | [@[[Brandon Toner](<../@[[Brandon Toner.md>)]] | [@[[Peter Rosso](<../@[[Peter Rosso.md>)]] | [@[[leekeifon](<../@[[leekeifon.md>)]] | [@[[Larissa de Lima](<../@[[Larissa de Lima.md>)]] | [@[[Samuel Bars](<../@[[Samuel Bars.md>)]] }}

# Backlinks
## [DNP Section](<DNP Section.md>)
- DNP Templates are found [here]([Graph/Templates](<../Graph/Templates.md>))

## [FAQ](<FAQ.md>)
- Check out [these]([Graph/Templates](<../Graph/Templates.md>))

## [January 25th, 2021](<January 25th, 2021.md>)
1. "[~](<../~.md>) [Brandon Toner](<../Brandon Toner.md>) how do you feel about using templates? I like these daily note headings — I think using either templates or smartblocks could be great to standardize structure..." Love templates, they help to facilitate structure — started some [here]([Graph/Templates](<../Graph/Templates.md>))

## [choice algorithm](<choice algorithm.md>)
- **[Tags](<../Tags.md>):** [Graph/Templates](<../Graph/Templates.md>)

## [page-status questions](<page-status questions.md>)
- **[Namespaces](<../Namespaces.md>):** `[Q:](<../Q:.md>)`
    - **[Graph/Templates](<../Graph/Templates.md>):**

## [roam/templates](<roam/templates.md>)
- **[Related](<../Related.md>):** [Graph/Templates](<../Graph/Templates.md>)

