- **[Tags](<../Tags.md>):** [Collections](<../Collections.md>)
- **[Related](<../Related.md>):** [roam/templates](<../roam/templates.md>)
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
        - [42Setting](<../42Setting.md>) LastWeek #[Week-10: 03-08-2021](<../Week-10: 03-08-2021.md>)
        - [42Setting](<../42Setting.md>) LastWkRaw Week-10: 03-08-2021
        - [42Setting](<../42Setting.md>) ThisWeek #[Week-11: 03-15-2021](<../Week-11: 03-15-2021.md>)
        - [42Setting](<../42Setting.md>) ThisWkRaw Week-11: 03-15-2021
        - [42Setting](<../42Setting.md>) NextWeek #[Week-12: 03-22-2021](<../Week-12: 03-22-2021.md>)
        - [42Setting](<../42Setting.md>) NextWkRaw Week-12: 03-22-2021
        - [42Setting](<../42Setting.md>) ThisMonth #[March 2021](<../March 2021.md>)
        - [42Setting](<../42Setting.md>) ThisMnthRaw March 2021
        - [42Setting](<../42Setting.md>) NextMonth #[April 2021](<../April 2021.md>)
        - [42Setting](<../42Setting.md>) NextMnthRaw April 2021
    - Getting Started
        - .rcGS — Getting Started  [42SmartBlock](<../42SmartBlock.md>) 
            - [,[,<%INPUT:What is your name or pseudonym?%>,],]%> {{word-count}}
                - **Welcome to Roam Collective!** 😃 
                - **Next Steps:**
                    - Create your personal page using this template - [Personal Page Template](((8BBipopP5))).
                    - Share some thoughts.
            - ---
        - .rcYOU — Personal Page [42SmartBlock](<../42SmartBlock.md>)
            - **[Tags](<../Tags.md>):** [People](<../People.md>) [Members](<../Members.md>)
                - **[About me](<../About me.md>):**
                    - **[Twitter](<../Twitter.md>):** [not-populated](<../not-populated.md>)
                    - **[Website](<../Website.md>):** [not-populated](<../not-populated.md>) 
                    - **[Location](<../Location.md>):** [not-populated](<../not-populated.md>)
                    - **[Time Zone](<../Time Zone.md>):** [not-populated](<../not-populated.md>)
                - **Online Status:**  {{or:⚫️Offline | 🟠Away | 🟡On & Off | 🟢Online}}
            - ---
            - **Personal SmartBlocks:**
                - .rcDNP <%CONCAT:<%INPUT:Your first initial and last name, or unique identifier%>%> — Daily Notes Template <%CONCAT:#,42SmartBlock%> <%CONCAT:#,roam/templates%>
                    - [,[,<%INPUT:What is your name or pseudonym?%>,],]%> {{word-count}}
                    - ---
    - Daily Templates
        - .rc2DH — Daily Header [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - #[Community Notes](<../Community Notes.md>) [Roam-Collective](<../Roam-Collective.md>) {{word-count}} [*]([rc](<../rc.md>)) 
                - #[Main Feed](<../Main Feed.md>) ((A place to showcase graph highlights throughout the day)) [not-populated](<../not-populated.md>) 
                - #[Graph Change Log](<../Graph Change Log.md>) [not-populated](<../not-populated.md>)
            - ---
        - .rc1DNP — Daily Notes Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - If this is your first time making a DNP section, use .gs instead.
            - If you are using this to routinely make a DNP section, create a custom one instead (use .YOU) 
            - ---
    - Quick Dates (uses the week & month format of the [Date Planner](<../Date Planner.md>))
        - .Today [42SmartBlock](<../42SmartBlock.md>)
            - <%DATE:today%>
        - .Tomorrow [42SmartBlock](<../42SmartBlock.md>)
            - <%DATE:tomorrow%>
        - .This Week [42SmartBlock](<../42SmartBlock.md>)
            - <%SET:dt,<%DATE:today,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%J:roam42.sb.vars["dt"]= dayjs(roam42.common.startOfWeek(new Date(roam42.sb.vars["dt"]))).format('MM-DD-YYYY')%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[Week-%><%GET:weekNum%>: <%GET:dt%>]]
        - .This Month [42SmartBlock](<../42SmartBlock.md>)
            - <%SET:dt,<%DATE:today,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[%><%DATE:<%GET:dt%>,MMMM YYYY%>]]
        - .Next Week [42SmartBlock](<../42SmartBlock.md>)
            - <%SET:dt,<%DATE:next week,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%J:roam42.sb.vars["dt"]= dayjs(roam42.common.startOfWeek(new Date(roam42.sb.vars["dt"]))).format('MM-DD-YYYY')%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[Week-%><%GET:weekNum%>: <%GET:dt%>]]
        - .Next Month [42SmartBlock](<../42SmartBlock.md>)
            - <%SET:dt,<%DATE:next month,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[%><%DATE:<%GET:dt%>,MMMM YYYY%>]]
        - .Insert WEEK Tag (input) [42SmartBlock](<../42SmartBlock.md>)
            - <%SET:dt,<%DATE:<%INPUT:Week of?%%Today%>,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%J:roam42.sb.vars["dt"]= dayjs(roam42.common.startOfWeek(new Date(roam42.sb.vars["dt"]))).format('MM-DD-YYYY')%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[Week-%><%GET:weekNum%>: <%GET:dt%>]]
        - .Insert MONTH Tag (input) [42SmartBlock](<../42SmartBlock.md>)
            - <%SET:dt,<%DATE:<%INPUT:Week of?%%Today%>,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[%><%DATE:<%GET:dt%>,MMMM YYYY%>]]
    - Productivity
        - .rc3GTD — Daily Review GTD [42SmartBlock](<../42SmartBlock.md>)
            - **[Daily Review](<../Daily Review.md>):**
                - **Scheduled for Today:**
                    - <%IFDAYOFWEEK:1,2%> [ ] Update week variables <%DATE:Today%>
                        - {{[embed](<../embed.md>): Global Variables}}
                    - <%IFDAYOFMONTH:1,2%> [ ] Update month variables <%DATE:Today%>
                        - {{[embed](<../embed.md>): Global Variables}}
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
    - Zettelkasten Queries 
        - Daily
            - Today + Obs [42SmartBlock](<../42SmartBlock.md>)
                - **Observations:**
                    - [min-title](<../min-title.md>) <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[Obs],] {not: [,[query]]}},},}%>
            - Today + Q [42SmartBlock](<../42SmartBlock.md>)
                - **Questions:** 
                    - [min-title](<../min-title.md>) <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[Q],] {not: [,[query]]}},},}%>
            - Today + I [42SmartBlock](<../42SmartBlock.md>)
                - **Ideas:**
                    - [min-title](<../min-title.md>) <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[I],] {not: [,[query]]}},},}%>
            - Today + FN [42SmartBlock](<../42SmartBlock.md>)
                - **Fleeting Notes:**
                    - [min-title](<../min-title.md>) <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[FN],] {not: [,[query]]}},},}%>
            - Today + LN [42SmartBlock](<../42SmartBlock.md>)
                - **Literature Notes:**
                    - [min-title](<../min-title.md>) <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[LN],] {not: [,[query]]}},},}%>
    - TODO Queries
        - Active Epics [42SmartBlock](<../42SmartBlock.md>)
            - **Active Epic(s):**
                - [page-focus](<../page-focus.md>) {{[query](<../query.md>): {and: [Epics](<../Epics.md>) [Status/Active](<../Status/Active.md>) {not: [query](<../query.md>)}}}}
        - Active Sprints [42SmartBlock](<../42SmartBlock.md>)
            - **Active Sprint(s):**
                - [page-focus](<../page-focus.md>) {{[query](<../query.md>): {and: [Sprints](<../Sprints.md>) [Status/Active](<../Status/Active.md>) {not: [query](<../query.md>)}}}}
        - TODO Created Today [42SmartBlock](<../42SmartBlock.md>)
            - **TODO Query:** (created today)
                - <%CONCAT:{,{[,[query],]: {and: <%DATE:today%> [,[TODO],]},},}%>
        - TODO + ThisWeek [42SmartBlock](<../42SmartBlock.md>)
            - **TODO Query:** (scheduled for this week)
                - <%CONCAT:{,{[,[query],]: {and: <%42SETTING:ThisWeek%> [,[TODO],]},},}%>
        - TODO + Help Wanted [42SmartBlock](<../42SmartBlock.md>)
            - **Help Wanted Query:**
                - [min-con](<../min-con.md>) <%CONCAT:{,{[,[query]]: {and: [,[Help Wanted]] [,[TODO]] {not: {or: [,[DONE]] [,[roam/css]]}}}},}%>
    - Change Log Query
        - Change Log + Today [42SmartBlock](<../42SmartBlock.md>)
            - <%CONCAT:#,min-title {,{[,[query]]: {and: <%DATE:today%> [,[Change Log]] {not: {or: [,[Community Notes]] [,[not-populated]]}}}}}%>
    - Page Templates
        - .rcPRJ — Projects Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Projects](<../Projects.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.Today}}
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
        - .rcREF — Reference Note Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Resources](<../Resources.md>) #[Reference Notes](<../Reference Notes.md>) ((add type of resource... Articles, Books, Videos etc.))
                - **[Author(s)](<../Author(s).md>):** [not-populated](<../not-populated.md>)
                - **[Full Title](<../Full Title.md>):** [not-populated](<../not-populated.md>)
                - **[URL](<../URL.md>):** [not-populated](<../not-populated.md>)
        - .rcCRT — Creative Project Template [42SmartBlock](<../42SmartBlock.md>) #[roam/templates](<../roam/templates.md>)
            - **[Tags](<../Tags.md>):** [Projects](<../Projects.md>) [Creative](<../Creative.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.Today}}
                - **[Resources](<../Resources.md>):** [not-populated](<../not-populated.md>)
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>)
                - **[Outline](<../Outline.md>):** [not-populated](<../not-populated.md>)
                - **[Next Steps](<../Next Steps.md>):** [not-populated](<../not-populated.md>) ((Plans for future elaboration or development))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
        - .rcSPR — Sprints Template [42SmartBlock](<../42SmartBlock.md>) #[roam/templates](<../roam/templates.md>)
            - **[Tags](<../Tags.md>):** [Sprints](<../Sprints.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.Today}}
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
                        - {{[query](<../query.md>): {and: [ex-A](<../ex-A.md>) {or: [E:](<../E:.md>) [N](<../N.md>) [I](<../I.md>) [Literature Notes](<../Literature Notes.md>)}}}} [minimal](<../minimal.md>)
                - **[Tasks](<../Tasks.md>):** [not-populated](<../not-populated.md>) ((Replace ex-A with the sprint page name))
                    - **[Query](<../Query.md>):** 
                        - {{[query](<../query.md>): {and: [ex-A](<../ex-A.md>) [TODO](<../TODO.md>)}}}
                - **[Work Summary](<../Work Summary.md>):** [not-populated](<../not-populated.md>) ((Include your name, the date, a description of the work, and a link to the work))
        - .rcEPC — Epics Template [42SmartBlock](<../42SmartBlock.md>) #[roam/templates](<../roam/templates.md>)
            - **[Tags](<../Tags.md>):** [Epics](<../Epics.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Date Range](<../Date Range.md>):** [not-populated](<../not-populated.md>)
                - **[Description](<../Description.md>):** [not-populated](<../not-populated.md>)
                - **[Status](<../Status.md>):** [not-populated](<../not-populated.md>)
                - **[Resources](<../Resources.md>):** [not-populated](<../not-populated.md>)
                - **[Work Summary](<../Work Summary.md>):** [not-populated](<../not-populated.md>) ((Include your name, the date, a description of the work, and a link to the work))
        - .rcEVN — Evergreen Note Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** #[Evergreens](<../Evergreens.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Author](<../Author.md>):** [not-populated](<../not-populated.md>)
                - **[References](<../References.md>):** [not-populated](<../not-populated.md>) ((Supporting FN, LN, EN, or RN would go here))
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>) ((Not a reference, but a related idea, block or page))
                - **[Next Steps](<../Next Steps.md>):** [not-populated](<../not-populated.md>) ((Plans for future elaboration or development))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
        - .rcMXM — Maxims Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Maxims](<../Maxims.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Author](<../Author.md>):** [not-populated](<../not-populated.md>)
                - **[Source](<../Source.md>):** [not-populated](<../not-populated.md>)
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>) ((Not a reference, but a related idea, block or page))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
        - .rcSDL — Seedlings Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Seedlings](<../Seedlings.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.Today}}
                - **[Created by](<../Created by.md>):** [not-populated](<../not-populated.md>)
                - **[Author](<../Author.md>):** [not-populated](<../not-populated.md>)
                - **[References](<../References.md>):** [not-populated](<../not-populated.md>) ((Supporting FN, LN, EN, or RN would go here))
                - **[Relevant Notes](<../Relevant Notes.md>):** [not-populated](<../not-populated.md>) ((Not a reference, but a related idea, block or page))
                - **[Next Steps](<../Next Steps.md>):** [not-populated](<../not-populated.md>) ((Plans for future elaboration or development))
                - **[Contents](<../Contents.md>):** [not-populated](<../not-populated.md>)
        - .rcQST — Questions Template [42SmartBlock](<../42SmartBlock.md>) [roam](<../roam.md>)/templates
            - **[Tags](<../Tags.md>):** [Questions](<../Questions.md>)
                - **[Date Created](<../Date Created.md>):** {{Today:42SmartBlock:.Today}}
                - **[Last Updated](<../Last Updated.md>):** {{Today:42SmartBlock:.Today}}
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
        - .rcNotify — @Everyone Tag  [42SmartBlock](<../42SmartBlock.md>)  [roam](<../roam.md>)/templates
            - {{or: [@[[Everyone](<../@[[Everyone.md>)]] | [@[[Charles Farr](<../@[[Charles Farr.md>)]] | [@[[Brandon Toner](<../@[[Brandon Toner.md>)]] | [@[[Peter Rosso](<../@[[Peter Rosso.md>)]] | [@[[leekeifon](<../@[[leekeifon.md>)]] | [@[[Larissa de Lima](<../@[[Larissa de Lima.md>)]] | [@[[Samuel Bars](<../@[[Samuel Bars.md>)]] }}

# Backlinks
## [Beyond the Basics](<Beyond the Basics.md>)
1. [~](<../~.md>) [Brandon Toner](<../Brandon Toner.md>) how do you feel about using templates? I like these daily note headings — I think using either templates or smartblocks could be great to standardize structure... Love templates, they help to facilitate structure — started some [here]([Graph/Templates](<../Graph/Templates.md>))

## [DNP Section](<DNP Section.md>)
- DNP Templates are found [here]([Graph/Templates](<../Graph/Templates.md>))

## [FAQ](<FAQ.md>)
- Check out [these]([Graph/Templates](<../Graph/Templates.md>))

## [January 25th, 2021](<January 25th, 2021.md>)
1. [~](<../~.md>) [Brandon Toner](<../Brandon Toner.md>) how do you feel about using templates? I like these daily note headings — I think using either templates or smartblocks could be great to standardize structure... Love templates, they help to facilitate structure — started some [here]([Graph/Templates](<../Graph/Templates.md>))

## [Matthew Vogel](<Matthew Vogel.md>)
- [Graph/Templates](<../Graph/Templates.md>)

## [My Daily Notes](<My Daily Notes.md>)
1. [~](<../~.md>) [Brandon Toner](<../Brandon Toner.md>) how do you feel about using templates? I like these daily note headings — I think using either templates or smartblocks could be great to standardize structure... Love templates, they help to facilitate structure — started some [here]([Graph/Templates](<../Graph/Templates.md>))

## [RC/Onboarding Seedpack](<RC/Onboarding Seedpack.md>)
- [Graph/Templates](<../Graph/Templates.md>)

## [Sidebar Archive: May 24th, 2021](<Sidebar Archive: May 24th, 2021.md>)
- [Graph/Templates](<../Graph/Templates.md>)

## [choice algorithm](<choice algorithm.md>)
- **[Tags](<../Tags.md>):** [Graph/Templates](<../Graph/Templates.md>)

## [page-status questions](<page-status questions.md>)
- **[Namespaces](<../Namespaces.md>):** `[Q:](<../Q:.md>)`
    - **[Graph/Templates](<../Graph/Templates.md>):**

## [roam/templates](<roam/templates.md>)
- **[Related](<../Related.md>):** [Graph/Templates](<../Graph/Templates.md>)

