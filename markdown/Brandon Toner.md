- Tags:: #People #Members #Moderators
    - About me::
        - Twitter:: [@brandontoner](https://twitter.com/brandontoner)
        - Website:: [brandontoner.substack.com](https://t.co/PQwCMbPZwT?amp=1)
        - Location:: [[Cape Breton]], [[Nova Scotia]] [[Canada]]
        - Time Zone:: [[Atlantic Time]] ([[UTC]] -4:00)
        - Birthday:: [[September 5th, 2021]] 
        - How to contact me:: 
            - Send me a DM on Roam Slack (preferred)
            - Send me a DM on Twitter (also great)
            - Tag me in something here ([under development, but YEA give it a hook — I'll see it]([[Chat]]))
    - {{or:🟡On & Off | 🟠Away | ⚫️Offline | 🟢Online}}
- **Personal Queries:**
    - Notifications
        - **Unread Notifications:**
            - {{[[query]]: {and: [[@[[Brandon Toner]]]] {not: [[query]]]}}}} #minimal
        - **CC'd Mentions:**
            - {{[[query]]: {and: [[cc:[[Brandon Toner]]]] {not: [[query]]]}}}} #minimal
    - My Daily Notes
        - **My Daily Notes:**
            - #min-con {{[[query]]: {and: [[Brandon Toner]] [[bnt]] {not: {or: [[query]] }}  }}}
    - Questions & Ideas
        - **Questions:**
            - #minimal {{[[query]]: {and: [[Brandon Toner]] [[Q]] [[bnt]] {not: {or: }}  }}}
        - **Ideas:**
            - #minimal {{[[query]]: {and: [[Brandon Toner]] [[I]] [[bnt]] {not: {or: }}  }}}
    - Zettelkasten Notes
        - **Fleeting Notes:**
            - #minimal {{[[query]]: {and: [[Brandon Toner]] [[N]] [[bnt]] {not: {or: }}  }}}
    - Productiviy
        - **Follow Ups:**
            - #minimal {{[[query]]: {and: [[Brandon Toner]] [[Follow Up]] [[bnt]] {not: {or: }}  }}}
        - **Todos:**
            - #minimal {{[[query]]: {and: [[Brandon Toner]] [[TODO]] {not: {or: [[query]] }}  }}}
- **Personal SmartBlocks:**
    - BToner -- .DNP Template #roam/templates #Graph/Templates
        - [[Brandon Toner]] {{word-count}} [*]([[bnt]])
            - [[Journal]]
            - [[Conversation & Comments]]
                - {{Pull Calls to Attention:42SmartBlock:BToner - Calls to Attention-Button:42RemoveButton=True}}
        - ---
    - Mentions (BT)
    - BToner — Andy's Notes #42SmartBlock #roam/templates
        - Tags:: #[[Evergreens]] #[[Reference Notes]] #[[Andy's Notes]]
            - Date Created:: {{Today:42SmartBlock:.Today}}
            - Created by:: [[Brandon Toner]]
            - Author:: [[Andy Matuschak]]
            - URL: #not-populated
            - References:: #not-populated ((Supporting FN, LN, EN, or RN would go here))
            - Related:: #not-populated ((Not a reference, but a related idea, block or page))
            - Contents:: #not-populated
    - TODO
        - BToner — My TODOs #42SmartBlock
            - **Ways you can help:**
                - **Results:** <%BLOCKMENTIONS:-1,TODO,Brandon Toner,-DONE,-query,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[[embed]]: <%BLOCKMENTIONS:20,TODO,Brandon Toner,-DONE,-query,-`%>}}
        - BToner — TODO + bnt #42SmartBlock
            - **TODOs:** (+ bnt)
                - <%CONCAT:#,minimal {,{[,[query]]: {and: [,[bnt]] [,[TODO]] {not: [,[query]]}}}}%>
        - BToner — TODO + Brandon Toner #42SmartBlock
            - **TODOs:** (+ Brandon Toner)
                - <%CONCAT:#,minimal {,{[,[query]]: {and: [,[Brandon Toner]] [,[TODO]] {not: [,[query]]}}}}%>
        - BToner — TODO + bnt + [today] #42SmartBlock
            - **TODOs:** (+ bnt (created today))
                - <%CONCAT:{,{[,[query],]: {and: [,[bnt],] <%DATE:today%> [,[TODO],]},},}%>
    - Zettelkasten Queries
        - BToner — Today + Obs + bnt #42SmartBlock
            - **Observations:**
                - #min-title <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[Obs],] {not: [,[query]]}},},}%>
        - BToner — Today + Q + bnt#42SmartBlock
            - **Questions:** 
                - #min-title <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[Q],] {not: [,[query]]}},},}%>
        - BToner — Today + I + bnt#42SmartBlock
            - **Ideas:**
                - #min-title <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[I],] {not: [,[query]]}},},}%>
        - BToner — Today + FN + bnt #42SmartBlock
            - **Fleeting Notes:**
                - #min-title <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[FN],] {not: [,[query]]}},},}%>
        - BToner — Today + LN + bnt #42SmartBlock
            - **Literature Notes:**
                - #min-title <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[LN],] {not: [,[query]]}},},}%>
    - BToner — ChatName #42SmartBlock #roam/templates
        - **Brandon:** 
    - BToner — @Charles #42SmartBlock #roam/templates
        - <%CONCAT:[@Charles]([,[@[,[Charles Farr]]]])%>
    - BToner — Chat banner UTC **+ Local** #42SmartBlock
        - Brandon Toner:: __<%J:return dayjs.utc().format("HH:mm") + " UTC" 
          + ' / ' + 
         dayjs().format("HH:mm ") +  new Date().toLocaleTimeString('en-us',{timeZoneName:'short'})  .split(' ')[2]%>__
    - BToner — Chat banner UTC **ONLY** #42SmartBlock
        - Brandon Toner:: __<%J:return dayjs.utc().format("HH:mm") + " UTC"%>__
    - BToner — Calls to Attention-Button #42SmartBlock 
        - re: [replace_this_text](<%BLOCKMENTIONS:20,@[[Brandon Toner]],-mentions%>)
        - {{Pull Calls to Attention:42SmartBlock:BToner - Calls to Attention-Button:42RemoveButton=True}}
    - **Archive**
        - BToner — .DNP Template (V1) 
            - #[[My Daily Notes]] [[Brandon Toner]] {{word-count}} [*]([[bnt]]) {{or:🟡On & Off | 🟠Away | ⚫️Offline | 🟢Online}}
                - #Scratchpad #not-populated
                - #[[Conversation & Comments]] #not-populated
                - #[[The Zettelkasten]]
                    - {{BToner — Today + Obs + bnt :42SmartBlock:BToner — Today + Obs + bnt}}
                    - {{BToner — Today + Q + bnt:42SmartBlock:BToner — Today + Q + bnt}}
                    - {{BToner — Today + I + bnt:42SmartBlock:BToner — Today + I + bnt}}
                    - {{BToner — Today + FN + bnt:42SmartBlock:BToner — Today + FN + bnt}}
                - #[[GTD Zone]]
                    - {{TODO + bnt:42SmartBlock:BToner — TODO + bnt}}
                    - {{TODO + bnt + createdtoday:42SmartBlock:BToner — TODO + bnt + [today]}}
                    - {{TODO + Brandon Toner:42SmartBlock:BToner — TODO + Brandon Toner}}
                - #[[Change Log]] #not-populated
            - ---
        - BToner — .DNP Template (V2)
            - #[[My Daily Notes]] [[Brandon Toner]] {{word-count}} [*]([[bnt]]) {{or:🟡On & Off | 🟠Away | ⚫️Offline | 🟢Online}}
                - #Scratchpad #not-populated
                - #[[Conversation & Comments]] #not-populated <%CURRENTBLOCKREF:newDNPRoot%>
                - #[[Change Log]] #not-populated
            - ---
            - <%SIDEBARWINDOWOPEN:<%GET:newDNPRoot%>%>
