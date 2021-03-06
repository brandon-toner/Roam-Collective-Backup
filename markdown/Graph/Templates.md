- Tags:: #Collections
- Related:: [[roam/templates]]
- Table of Contents::
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
- Contents::
    - Global Variables
        - #42Setting LastWeek #[[Week-10: 03-08-2021]]
        - #42Setting LastWkRaw Week-10: 03-08-2021
        - #42Setting ThisWeek #[[Week-11: 03-15-2021]]
        - #42Setting ThisWkRaw Week-11: 03-15-2021
        - #42Setting NextWeek #[[Week-12: 03-22-2021]]
        - #42Setting NextWkRaw Week-12: 03-22-2021
        - #42Setting ThisMonth #[[March 2021]]
        - #42Setting ThisMnthRaw March 2021
        - #42Setting NextMonth #[[April 2021]]
        - #42Setting NextMnthRaw April 2021
    - Getting Started
        - .rcGS — Getting Started  #42SmartBlock 
            - [,[,<%INPUT:What is your name or pseudonym?%>,],]%> {{word-count}}
                - **Welcome to Roam Collective!** 😃 
                - **Next Steps:**
                    - Create your personal page using this template - [Personal Page Template](((8BBipopP5))).
                    - Share some thoughts.
            - ---
        - .rcYOU — Personal Page #42SmartBlock
            - Tags:: #People #Members
                - About me::
                    - Twitter:: #not-populated
                    - Website:: #not-populated 
                    - Location:: #not-populated
                    - Time Zone:: #not-populated
                - **Online Status:**  {{or:⚫️Offline | 🟠Away | 🟡On & Off | 🟢Online}}
            - ---
            - **Personal SmartBlocks:**
                - .rcDNP <%CONCAT:<%INPUT:Your first initial and last name, or unique identifier%>%> — Daily Notes Template <%CONCAT:#,42SmartBlock%> <%CONCAT:#,roam/templates%>
                    - [,[,<%INPUT:What is your name or pseudonym?%>,],]%> {{word-count}}
                    - ---
    - Daily Templates
        - .rc2DH — Daily Header #42SmartBlock #roam/templates
            - #[[Community Notes]] [[Roam-Collective]] {{word-count}} [*]([[rc]]) 
                - #[[Main Feed]] ((A place to showcase graph highlights throughout the day)) #not-populated 
                - #[[Graph Change Log]] #not-populated
            - ---
        - .rc1DNP — Daily Notes Template #42SmartBlock #roam/templates
            - If this is your first time making a DNP section, use .gs instead.
            - If you are using this to routinely make a DNP section, create a custom one instead (use .YOU) 
            - ---
    - Quick Dates (uses the week & month format of the [[Date Planner]])
        - .Today #42SmartBlock
            - <%DATE:today%>
        - .Tomorrow #42SmartBlock
            - <%DATE:tomorrow%>
        - .This Week #42SmartBlock
            - <%SET:dt,<%DATE:today,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%J:roam42.sb.vars["dt"]= dayjs(roam42.common.startOfWeek(new Date(roam42.sb.vars["dt"]))).format('MM-DD-YYYY')%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[Week-%><%GET:weekNum%>: <%GET:dt%>]]
        - .This Month #42SmartBlock
            - <%SET:dt,<%DATE:today,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[%><%DATE:<%GET:dt%>,MMMM YYYY%>]]
        - .Next Week #42SmartBlock
            - <%SET:dt,<%DATE:next week,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%J:roam42.sb.vars["dt"]= dayjs(roam42.common.startOfWeek(new Date(roam42.sb.vars["dt"]))).format('MM-DD-YYYY')%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[Week-%><%GET:weekNum%>: <%GET:dt%>]]
        - .Next Month #42SmartBlock
            - <%SET:dt,<%DATE:next month,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[%><%DATE:<%GET:dt%>,MMMM YYYY%>]]
        - .Insert WEEK Tag (input) #42SmartBlock
            - <%SET:dt,<%DATE:<%INPUT:Week of?%%Today%>,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%J:roam42.sb.vars["dt"]= dayjs(roam42.common.startOfWeek(new Date(roam42.sb.vars["dt"]))).format('MM-DD-YYYY')%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[Week-%><%GET:weekNum%>: <%GET:dt%>]]
        - .Insert MONTH Tag (input) #42SmartBlock
            - <%SET:dt,<%DATE:<%INPUT:Week of?%%Today%>,MM-DD-YYYY%>%><%NOBLOCKOUTPUT%>
            - <%SET:weekNum,<%J:return dayjs(roam42.sb.vars["dt"]).week()-1%>%> <%NOBLOCKOUTPUT%>
            - <%CONCAT:#,[,[%><%DATE:<%GET:dt%>,MMMM YYYY%>]]
    - Productivity
        - .rc3GTD — Daily Review GTD #42SmartBlock
            - Daily Review::
                - **Scheduled for Today:**
                    - <%IFDAYOFWEEK:1,2%> {{[[TODO]]}} Update week variables <%DATE:Today%>
                        - {{[[embed]]: Global Variables}}
                    - <%IFDAYOFMONTH:1,2%> {{[[TODO]]}} Update month variables <%DATE:Today%>
                        - {{[[embed]]: Global Variables}}
                    - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:20,TODO,<%DATE:today%>,-DONE%>}}
                - {{Overdue:42SmartBlock:.rc3TODO — TODO Overdue (10, with header)}}
                - {{Flagged:42SmartBlock:.rc4FLG — Flagged}}
                - {{Waiting:42SmartBlock:.rc3WAIT — Waiting}}
                - {{TODO This Week:42SmartBlock:.rc3TODO — TODO This Week}}
                - {{TODO This Month:42SmartBlock:.rc3TODO — TODO This Month}}
            - **Ways you can help:**
                - __Check out the linked references on the Help Wanted tag for more other ways you can contribute.__ Thanks for being here 😄
                - **Results:** <%BLOCKMENTIONS:-1,TODO,Help Wanted,-DONE,-query,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:20,TODO,Help Wanted,-DONE,-query,-`%>}}
        - .rc4FLG — Flagged #42SmartBlock
            - **Flagged:**
                - **Results:** <%BLOCKMENTIONS:-1,Flagged,-query,-DONE,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:20,Flagged,-query,-DONE,-`%>}}
        - .rc3WAIT — Waiting #42SmartBlock
            - **Waiting:**
                - **Results:** <%BLOCKMENTIONS:-1,Waiting,-DONE,-query,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:20,Waiting,-DONE,-query,-`%>}}
        - .rc3TODO — Scheduled for Today #42SmartBlock
            - **Scheduled for Today:**
                - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:20,TODO,<%DATE:today%>,-DONE%>}}
        - .rc3TODO — TODO Overdue (10, with header) #42SmartBlock
            - **Overdue TODOs:**  
                - {{[[embed]]: <%TODOOVERDUE:10%>}}
        - .rc3TODO — TODO This Week #42SmartBlock 
            - **This Week:** `<%42SETTING:ThisWeek%>`
                - **Results:** <%BLOCKMENTIONS:-1,TODO,<%42SETTING:ThisWkRaw%>,-DONE%> **Max:** 25
                - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:25,TODO,<%42SETTING:ThisWkRaw%>,-DONE%>}}
        - .rc3TODO — TODO This Month #42SmartBlock
            - **This Month:** `<%42SETTING:ThisMonth%>`
                - **Results:** <%BLOCKMENTIONS:-1,TODO,<%42SETTING:ThisMnthRaw%>,-DONE%> **Max:** 25
                - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:25,TODO,<%42SETTING:ThisMnthRaw%>,-DONE%>}}
        - .rc3TODO — TODO Help Wanted #42SmartBlock
            - **Ways you can help:**
                - __Check out the linked references on the Help Wanted tag for more other ways you can contribute.__ Thanks for being here 😄
                - **Results:** <%BLOCKMENTIONS:-1,TODO,Help Wanted,-DONE,-query,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:20,TODO,Help Wanted,-DONE,-query,-`%>}}
    - Zettelkasten Queries 
        - Daily
            - Today + Obs #42SmartBlock
                - **Observations:**
                    - #min-title <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[Obs],] {not: [,[query]]}},},}%>
            - Today + Q #42SmartBlock
                - **Questions:** 
                    - #min-title <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[Q],] {not: [,[query]]}},},}%>
            - Today + I #42SmartBlock
                - **Ideas:**
                    - #min-title <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[I],] {not: [,[query]]}},},}%>
            - Today + FN #42SmartBlock
                - **Fleeting Notes:**
                    - #min-title <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[FN],] {not: [,[query]]}},},}%>
            - Today + LN #42SmartBlock
                - **Literature Notes:**
                    - #min-title <%CONCAT:{,{[,[query],]: {and: %><%DATE:today%> <%CONCAT:[,[LN],] {not: [,[query]]}},},}%>
    - TODO Queries
        - Active Epics #42SmartBlock
            - **Active Epic(s):**
                - #page-focus {{[[query]]: {and: [[Epics]] [[Status/Active]] {not: [[query]]}}}}
        - Active Sprints #42SmartBlock
            - **Active Sprint(s):**
                - #page-focus {{[[query]]: {and: [[Sprints]] [[Status/Active]] {not: [[query]]}}}}
        - TODO Created Today #42SmartBlock
            - **TODO Query:** (created today)
                - <%CONCAT:{,{[,[query],]: {and: <%DATE:today%> [,[TODO],]},},}%>
        - TODO + ThisWeek #42SmartBlock
            - **TODO Query:** (scheduled for this week)
                - <%CONCAT:{,{[,[query],]: {and: <%42SETTING:ThisWeek%> [,[TODO],]},},}%>
        - TODO + Help Wanted #42SmartBlock
            - **Help Wanted Query:**
                - #min-con <%CONCAT:{,{[,[query]]: {and: [,[Help Wanted]] [,[TODO]] {not: {or: [,[DONE]] [,[roam/css]]}}}},}%>
    - Change Log Query
        - Change Log + Today #42SmartBlock
            - <%CONCAT:#,min-title {,{[,[query]]: {and: <%DATE:today%> [,[Change Log]] {not: {or: [,[Community Notes]] [,[not-populated]]}}}}}%>
    - Page Templates
        - .rcPRJ — Projects Template #42SmartBlock #roam/templates
            - Tags:: #Projects
                - Date Created:: {{Today:42SmartBlock:.Today}}
                - Related:: #[[not-populated]]
                - People:: #[[not-populated]] #Housekeeping
                    - Created by:: #not-populated
                    - Project Lead:: #not-populated
                    - Contributors:: #not-populated
                - Areas:: #[[not-populated]] #Housekeeping
                - Project Status:: #[[not-populated]] #Housekeeping
                - Due Date:: #[[not-populated]] #Housekeeping
                - Reminders:: #[[not-populated]] 
                - Date Completed:: #[[Status/Not Completed]]
                - Notes:: #[[not-populated]]
                - Tasks:: #not-populated
        - .rcREF — Reference Note Template #42SmartBlock #roam/templates
            - Tags:: #Resources #[[Reference Notes]] ((add type of resource... Articles, Books, Videos etc.))
                - Author(s):: #not-populated
                - Full Title:: #not-populated
                - URL:: #not-populated
        - .rcCRT — Creative Project Template #42SmartBlock #[[roam/templates]]
            - Tags:: #Projects #Creative
                - Date Created:: {{Today:42SmartBlock:.Today}}
                - Last Updated:: {{Today:42SmartBlock:.Today}}
                - Resources:: #not-populated
                - Relevant Notes:: #not-populated
                - Outline:: #not-populated
                - Next Steps:: #not-populated ((Plans for future elaboration or development))
                - Contents:: #not-populated
        - .rcSPR — Sprints Template #42SmartBlock #[[roam/templates]]
            - Tags:: #Sprints
                - Date Created:: {{Today:42SmartBlock:.Today}}
                - Date Range:: #not-populated
                - Description:: #not-populated
                - Status:: #not-populated
                - Resources:: #not-populated
                - **Outlines:** #not-populated ((Replace ex-A with the sprint page name))
                    - Query::
                        - {{[[query]]: {and: [[ex-A]] [[Outlines]]}}} #minimal
                - **Questions:** #not-populated ((Replace ex-A with the sprint page name))
                    - Query::
                        - {{[[query]]: {and: [[ex-A]] {or: [[Q]] [[Questions]]}}}} #minimal
                - Relevant Notes:: #not-populated ((Replace ex-A with the sprint page name))
                    - Query::
                        - {{[[query]]: {and: [[ex-A]] {or: [[E:]] [[N]] [[I]] [[Literature Notes]]}}}} #minimal
                - Tasks:: #not-populated ((Replace ex-A with the sprint page name))
                    - Query:: 
                        - {{[[query]]: {and: [[ex-A]] [[TODO]]}}}
                - Work Summary:: #not-populated ((Include your name, the date, a description of the work, and a link to the work))
        - .rcEPC — Epics Template #42SmartBlock #[[roam/templates]]
            - Tags:: #Epics
                - Date Created:: {{Today:42SmartBlock:.Today}}
                - Created by:: #not-populated
                - Date Range:: #not-populated
                - Description:: #not-populated
                - Status:: #not-populated
                - Resources:: #not-populated
                - Work Summary:: #not-populated ((Include your name, the date, a description of the work, and a link to the work))
        - .rcEVN — Evergreen Note Template #42SmartBlock #roam/templates
            - Tags:: #[[Evergreens]]
                - Date Created:: {{Today:42SmartBlock:.Today}}
                - Last Updated:: {{Today:42SmartBlock:.Today}}
                - Created by:: #not-populated
                - Author:: #not-populated
                - References:: #not-populated ((Supporting FN, LN, EN, or RN would go here))
                - Relevant Notes:: #not-populated ((Not a reference, but a related idea, block or page))
                - Next Steps:: #not-populated ((Plans for future elaboration or development))
                - Contents:: #not-populated
        - .rcMXM — Maxims Template #42SmartBlock #roam/templates
            - Tags:: #Maxims
                - Date Created:: {{Today:42SmartBlock:.Today}}
                - Last Updated:: {{Today:42SmartBlock:.Today}}
                - Created by:: #not-populated
                - Author:: #not-populated
                - Source:: #not-populated
                - Relevant Notes:: #not-populated ((Not a reference, but a related idea, block or page))
                - Contents:: #not-populated
        - .rcSDL — Seedlings Template #42SmartBlock #roam/templates
            - Tags:: #Seedlings
                - Date Created:: {{Today:42SmartBlock:.Today}}
                - Last Updated:: {{Today:42SmartBlock:.Today}}
                - Created by:: #not-populated
                - Author:: #not-populated
                - References:: #not-populated ((Supporting FN, LN, EN, or RN would go here))
                - Relevant Notes:: #not-populated ((Not a reference, but a related idea, block or page))
                - Next Steps:: #not-populated ((Plans for future elaboration or development))
                - Contents:: #not-populated
        - .rcQST — Questions Template #42SmartBlock #roam/templates
            - Tags:: #Questions
                - Date Created:: {{Today:42SmartBlock:.Today}}
                - Last Updated:: {{Today:42SmartBlock:.Today}}
                - Created by:: #not-populated
                - Author:: #not-populated
                - Relevant Notes:: #not-populated ((Related notes in the graph — FN, LN, EN, Q, I, etc.))
                - Next Steps:: #not-populated ((Plans for future elaboration or development))
                - Contents:: #not-populated
                - Work Summary:: #not-populated ((Link to work related to this page from elsewhere in the graph — Include name & date if relevant))
    - Algorithms of Thought
        - .rc3CH — Choice AoT #roam/templates
            - {{[[TODO]]}} [[Choice]]:  ((((e-lL4buZ1))))
                - Options:: #not-populated
                - Status:: #not-populated
                - Decision:: #not-populated
                - Notes:: #not-populated
        - .rc3CH — Choice Options #42SmartBlock #roam/templates
            - <%INPUT:Letter (e.g. A, B, C)%%A%> -
                - Pros:: #not-populated
                - Cons:: #not-populated
    - Randomization 
        - .rc3RFN — Random Fleeting Note (Experimental) #42SmartBlock ((Not truly random...))
            - ^^Reminder:^^ __Please delete any block references where you did not add any annotations to prevent "empty references"__
            - **Page:** `<%PAGE%>`
<%BLOCKMENTIONS:<%INPUT:How may would you like to return?%%3%>,Fleeting Notes%>
        - .rc3RFN — Random Fleeting Note (Experimental) (no instructions) #42SmartBlock ((Not truly random...))
            - **Page:** `<%PAGE%>`
<%BLOCKMENTIONS:<%INPUT:How may would you like to return?%%3%>,Fleeting Notes%>
        - .rc3RSL — Random Seedling (Experimental) #42SmartBlock ((Not truly random...))
            - ^^Reminder:^^ __Please delete any block references where you did not add any annotations to prevent "empty references"__
            - **Page:** `<%PAGE%>`
<%BLOCKMENTIONS:<%INPUT:How may would you like to return?%%3%>,Seedlings%> 
        - .rc3RSL — Random Seedling (no instructions) (Experimental) #42SmartBlock ((Not truly random...))
            - **Page:** `<%PAGE%>`
<%BLOCKMENTIONS:<%INPUT:How may would you like to return?%%3%>,Seedlings%> 
        - ,rcREN — Random Evergreen Note (Experimental) #42SmartBlock
            - ^^Reminder:^^ __Please delete any block references where you did not add any annotations to prevent "empty references"__ ((The block reference generated is not important, that can be deleted.))
            - <%PAGE%>
((<%BLOCKMENTIONS:1,Evergreen Notes,Tags%>)) 
        - ,rcREN — Random Evergreen Note (no instructions) (Experimental) #42SmartBlock
            - <%PAGE%>
((<%BLOCKMENTIONS:1,Evergreen Notes,Tags%>)) 
    - Miscellaneous
        - .rc2CSS — Add to CSS #42SmartBlock #roam/templates
            - {{[[TODO]]}} Add to [[roam/css]]
        - ,rcTEN — "in tension with" #42SmartBlock #roam/templates
            - in [tension]([[Tensions]]) with
        - .rc1BRK — Horizontal Rule #42SmartBlock #roam/templates
            - ---
        - .rcDRP — Dropdown Menu #42SmartBlock #roam/templates
            - {{or: Option A | Option B | Option C}}
        - .rcBRB — Online/Status #42SmartBlock #roam/templates
            - {{or:🟢Online | 😴 offline, back tomorrow | 🟠Away}}
        - .rcNotify — @Everyone Tag  #42SmartBlock  #roam/templates
            - {{or: [[@[[Everyone]]]] | [[@[[Charles Farr]]]] | [[@[[Brandon Toner]]]] | [[@[[Peter Rosso]]]] | [[@[[leekeifon]]]] | [[@[[Larissa de Lima]]]] | [[@[[Samuel Bars]]]] }}
