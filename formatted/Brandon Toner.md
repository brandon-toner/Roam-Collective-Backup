- **[Tags](<Tags.md>):** [People](<People.md>) [Members](<Members.md>) [Moderators](<Moderators.md>)
    - **[About me](<About me.md>):**
        - **[Twitter](<Twitter.md>):** [@brandontoner](https://twitter.com/brandontoner)
        - **[Website](<Website.md>):** [brandontoner.substack.com](https://t.co/PQwCMbPZwT?amp=1)
        - **[Location](<Location.md>):** [Cape Breton](<Cape Breton.md>), [Nova Scotia](<Nova Scotia.md>) [Canada](<Canada.md>)
        - **[Time Zone](<Time Zone.md>):** [Atlantic Time](<Atlantic Time.md>) ([UTC](<UTC.md>) -4:00)
        - **[Birthday](<Birthday.md>):** [September 5th, 2021](<September 5th, 2021.md>) 
        - **[How to contact me](<How to contact me.md>):** 
            - Send me a DM on Roam Slack (preferred)
            - Send me a DM on Twitter (also great)
            - Tag me in something here ([under development, but YEA give it a hook — I'll see it]([Chat](<Chat.md>)))
    - {{or:🟡On & Off | 🟠Away | ⚫️Offline | 🟢Online}}
- **Personal Queries:**
    - Notifications
        - **Unread Notifications:**
            - {{[query](<query.md>): {and: [@[[Brandon Toner](<@[[Brandon Toner.md>)]] {not: [query](<query.md>)]}}}} [minimal](<minimal.md>)
        - **CC'd Mentions:**
            - {{[query](<query.md>): {and: [cc:[[Brandon Toner](<cc:[[Brandon Toner.md>)]] {not: [query](<query.md>)]}}}} [minimal](<minimal.md>)
    - My Daily Notes
        - **My Daily Notes:**
            - [min-con](<min-con.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>) [bnt](<bnt.md>) {not: {or: [query](<query.md>) }}  }}}
    - Questions & Ideas
        - **Questions:**
            - [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>) [Q](<Q.md>) [bnt](<bnt.md>) {not: {or: }}  }}}
        - **Ideas:**
            - [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>) [I](<I.md>) [bnt](<bnt.md>) {not: {or: }}  }}}
    - Zettelkasten Notes
        - **Fleeting Notes:**
            - [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>) [N](<N.md>) [bnt](<bnt.md>) {not: {or: }}  }}}
    - Productiviy
        - **Follow Ups:**
            - [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>) [Follow Up](<Follow Up.md>) [bnt](<bnt.md>) {not: {or: }}  }}}
        - **Todos:**
            - [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>) [TODO](<TODO.md>) {not: {or: [query](<query.md>) }}  }}}
- **Personal SmartBlocks:**
    - BToner — .DNP Template [42SmartBlock](<42SmartBlock.md>)
        - #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>) {{word-count}} [*]([bnt](<bnt.md>)) "{{or:🟡On & Off | 🟠Away | ⚫️Offline | 🟢Online}}"
            - [Scratchpad](<Scratchpad.md>) [not-populated](<not-populated.md>)
            - [Conversation](<Conversation.md>) [not-populated](<not-populated.md>) <%CURRENTBLOCKREF:newDNPRoot%>
            - #[Change Log](<Change Log.md>) [not-populated](<not-populated.md>)
        - ---
        - <%SIDEBARWINDOWOPEN:<%GET:newDNPRoot%>%>
    - Mentions (BT)
    - BToner — Andy's Notes [42SmartBlock](<42SmartBlock.md>) [roam](<roam.md>)/templates
        - **[Tags](<Tags.md>):** #[Evergreens](<Evergreens.md>) #[Reference Notes](<Reference Notes.md>) #[Andy's Notes](<Andy's Notes.md>)
            - **[Date Created](<Date Created.md>):** {{Today:42SmartBlock:.Today}}
            - **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)
            - **[Author](<Author.md>):** [Andy Matuschak](<Andy Matuschak.md>)
            - URL: [not-populated](<not-populated.md>)
            - **[References](<References.md>):** [not-populated](<not-populated.md>) ((Supporting FN, LN, EN, or RN would go here))
            - **[Related](<Related.md>):** [not-populated](<not-populated.md>) ((Not a reference, but a related idea, block or page))
            - **[Contents](<Contents.md>):** [not-populated](<not-populated.md>)
    - TODO
        - BToner — My TODOs [42SmartBlock](<42SmartBlock.md>)
            - **Ways you can help:**
                - **Results:** <%BLOCKMENTIONS:-1,TODO,Brandon Toner,-DONE,-query,-`%> **Max:** 20
                - **Page:** <%PAGE%>
{{[embed](<embed.md>): <%BLOCKMENTIONS:20,TODO,Brandon Toner,-DONE,-query,-`%>}}
        - BToner — TODO + bnt [42SmartBlock](<42SmartBlock.md>)
            - **TODOs:** (+ bnt)
                - <%CONCAT:#,minimal {,{[,[query]]: {and: [,[bnt]] [,[TODO]] {not: [,[query]]}}}}%>
        - BToner — TODO + Brandon Toner [42SmartBlock](<42SmartBlock.md>)
            - **TODOs:** (+ Brandon Toner)
                - <%CONCAT:#,minimal {,{[,[query]]: {and: [,[Brandon Toner]] [,[TODO]] {not: [,[query]]}}}}%>
        - BToner — TODO + bnt + [today] [42SmartBlock](<42SmartBlock.md>)
            - **TODOs:** (+ bnt (created today))
                - <%CONCAT:{,{[,[query],]: {and: [,[bnt],] <%DATE:today%> [,[TODO],]},},}%>
    - Zettelkasten Queries
        - BToner — Today + Obs + bnt [42SmartBlock](<42SmartBlock.md>)
            - **Observations:**
                - [min-title](<min-title.md>) <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[Obs],] {not: [,[query]]}},},}%>
        - BToner — Today + Q + bnt[42SmartBlock](<42SmartBlock.md>)
            - **Questions:** 
                - [min-title](<min-title.md>) <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[Q],] {not: [,[query]]}},},}%>
        - BToner — Today + I + bnt[42SmartBlock](<42SmartBlock.md>)
            - **Ideas:**
                - [min-title](<min-title.md>) <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[I],] {not: [,[query]]}},},}%>
        - BToner — Today + FN + bnt [42SmartBlock](<42SmartBlock.md>)
            - **Fleeting Notes:**
                - [min-title](<min-title.md>) <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[FN],] {not: [,[query]]}},},}%>
        - BToner — Today + LN + bnt [42SmartBlock](<42SmartBlock.md>)
            - **Literature Notes:**
                - [min-title](<min-title.md>) <%CONCAT:{,{[,[query],]: {and: [,[bnt]]%><%DATE:today%> <%CONCAT:[,[LN],] {not: [,[query]]}},},}%>
    - BToner — ChatName [42SmartBlock](<42SmartBlock.md>) [roam](<roam.md>)/templates
        - **Brandon:** 
    - BToner — @Charles [42SmartBlock](<42SmartBlock.md>) [roam](<roam.md>)/templates
        - <%CONCAT:[@Charles]([,[@[,[Charles Farr]]]])%>
    - BToner — Chat banner UTC **+ Local** [42SmartBlock](<42SmartBlock.md>)
        - **[Brandon Toner](<Brandon Toner.md>):** __<%J:return dayjs.utc().format("HH:mm") + " UTC" 
          + ' / ' + 
         dayjs().format("HH:mm ") +  new Date().toLocaleTimeString('en-us',{timeZoneName:'short'})  .split(' ')[2]%>__
    - BToner — Chat banner UTC **ONLY** [42SmartBlock](<42SmartBlock.md>)
        - **[Brandon Toner](<Brandon Toner.md>):** __<%J:return dayjs.utc().format("HH:mm") + " UTC"%>__
    - BToner — Calls to Attention-Button [42SmartBlock](<42SmartBlock.md>) 
        - re: [replace_this_text](<%BLOCKMENTIONS:20,@[Brandon Toner](<Brandon Toner.md>),-mentions%>)
        - {{Pull Calls to Attention:42SmartBlock:BToner - Calls to Attention-Button:42RemoveButton=True}}
    - **Archive**
        - BToner — .DNP Template (V1) 
            - #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>) {{word-count}} [*]([bnt](<bnt.md>)) "{{or:🟡On & Off | 🟠Away | ⚫️Offline | 🟢Online}}"
                - [Scratchpad](<Scratchpad.md>) [not-populated](<not-populated.md>)
                - [Conversation](<Conversation.md>) [not-populated](<not-populated.md>)
                - #[The Zettelkasten](<The Zettelkasten.md>)
                    - {{BToner — Today + Obs + bnt :42SmartBlock:BToner — Today + Obs + bnt}}
                    - {{BToner — Today + Q + bnt:42SmartBlock:BToner — Today + Q + bnt}}
                    - {{BToner — Today + I + bnt:42SmartBlock:BToner — Today + I + bnt}}
                    - {{BToner — Today + FN + bnt:42SmartBlock:BToner — Today + FN + bnt}}
                - #[GTD Zone](<GTD Zone.md>)
                    - {{TODO + bnt:42SmartBlock:BToner — TODO + bnt}}
                    - {{TODO + bnt + createdtoday:42SmartBlock:BToner — TODO + bnt + [today]}}
                    - {{TODO + Brandon Toner:42SmartBlock:BToner — TODO + Brandon Toner}}
                - #[Change Log](<Change Log.md>) [not-populated](<not-populated.md>)
            - ---

# Backlinks
## ["many hands make light work"](<"many hands make light work".md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [12 Favorite Problems](<12 Favorite Problems.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Abandon ideology.](<Abandon ideology..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [About Roam Collective](<About Roam Collective.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Act so that you can tell the truth about how you act.](<Act so that you can tell the truth about how you act..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Administration](<Administration.md>)
- **[Administrator](<Administrator.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Editor](<Editor.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Announcements](<Announcements.md>)
- **Jump right in!** [I'll]([Brandon Toner](<Brandon Toner.md>))

## [Ask someone to do you a small favour, so that he or she can ask you to do one in the future.](<Ask someone to do you a small favour, so that he or she can ask you to do one in the future..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Assume the person you are listening to might know something you don't.](<Assume the person you are listening to might know something you don't..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Be careful who you share bad news with.](<Be careful who you share bad news with..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Be careful who you share good news with.](<Be careful who you share good news with..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Be grateful in spite of your suffering.](<Be grateful in spite of your suffering..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Be precise in your speech.](<Be precise in your speech..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Brandon Toner](<Brandon Toner.md>)
- [min-con](<min-con.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>)

- [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>)

- [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>)

- [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>)

- [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>)

- [minimal](<minimal.md>) {{[query](<query.md>): {and: [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- BToner — Chat banner UTC **+ Local** [42SmartBlock](<42SmartBlock.md>)
        - **[Brandon Toner](<Brandon Toner.md>):**

- BToner — Chat banner UTC **ONLY** [42SmartBlock](<42SmartBlock.md>)
        - **[Brandon Toner](<Brandon Toner.md>):**

- re: [replace_this_text](<%BLOCKMENTIONS:20,@[Brandon Toner](<Brandon Toner.md>),

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [Compare yourself to who you were yesterday, not who someone else is today.](<Compare yourself to who you were yesterday, not who someone else is today..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [DNP Section](<DNP Section.md>)
- "#[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [Do not allow yourself to become arrogant or resentful.](<Do not allow yourself to become arrogant or resentful..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Do not bother children when they are skateboarding.](<Do not bother children when they are skateboarding..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Do not carelessly denigrate social institutions or artistic achievement.](<Do not carelessly denigrate social institutions or artistic achievement..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Do not do what you hate.](<Do not do what you hate..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Do not hide unwanted things in the fog.](<Do not hide unwanted things in the fog..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Do not let your children do anything that makes you dislike them.](<Do not let your children do anything that makes you dislike them..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Do not transform your wife into a maid.](<Do not transform your wife into a maid..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Do not try to rescue someone who does not want to be rescued, and be very careful about rescuing someone who does.](<Do not try to rescue someone who does not want to be rescued, and be very careful about rescuing someone who does..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Don't avoid something frightening if it stands in your way -- and don't do unnecessarily dangerous things.](<Don't avoid something frightening if it stands in your way -- and don't do unnecessarily dangerous things..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Don't let bullies get away with it.](<Don't let bullies get away with it..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Dress like the person you want to be.](<Dress like the person you want to be..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [E/Evergreen Note example 2](<E/Evergreen Note example 2.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Epics/Establish and document baseline RC conventions and workflows](<Epics/Establish and document baseline RC conventions and workflows.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/"Hacked" solutions are likely to break over time.](<Evergreens/"Hacked" solutions are likely to break over time..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Cite shared principles to foster alignment.](<Evergreens/Cite shared principles to foster alignment..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Claim 1](<Evergreens/Claim 1.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Create speculative outlines while you write](<Evergreens/Create speculative outlines while you write.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Documenting ideas in zettelkasten format promotes referencing in related contexts](<Evergreens/Documenting ideas in zettelkasten format promotes referencing in related contexts.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Evergreen Note example 3](<Evergreens/Evergreen Note example 3.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Evergreen note titles are like APIs](<Evergreens/Evergreen note titles are like APIs.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Evergreen note-writing helps insight accumulate](<Evergreens/Evergreen note-writing helps insight accumulate.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Evergreen notes should be atomic](<Evergreens/Evergreen notes should be atomic.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Evergreen notes should be concept-oriented](<Evergreens/Evergreen notes should be concept-oriented.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Evergreen notes should be densely linked](<Evergreens/Evergreen notes should be densely linked.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Have a clear aim](<Evergreens/Have a clear aim.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/How do you eat an elephant?](<Evergreens/How do you eat an elephant?.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Make evergreen notes as you write.](<Evergreens/Make evergreen notes as you write..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Make it work, then make it fast, then make it pretty.](<Evergreens/Make it work, then make it fast, then make it pretty..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Prefer note titles with complete phrases to sharpen claims](<Evergreens/Prefer note titles with complete phrases to sharpen claims.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Ready, Fire, Aim](<Evergreens/Ready, Fire, Aim.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Spaced repetition may be a helpful tool to incrementally develop inklings](<Evergreens/Spaced repetition may be a helpful tool to incrementally develop inklings.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Spaced repetition systems can be used to program attention](<Evergreens/Spaced repetition systems can be used to program attention.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Start from abundance](<Evergreens/Start from abundance.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/Use the native convention as much as possible.](<Evergreens/Use the native convention as much as possible..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/active vs passive resurfacing](<Evergreens/active vs passive resurfacing.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/alert fatigue](<Evergreens/alert fatigue.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/barrier to entry](<Evergreens/barrier to entry.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/beneficial, but optional](<Evergreens/beneficial, but optional.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/build once, sell twice](<Evergreens/build once, sell twice.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/cycles of divergence and convergence](<Evergreens/cycles of divergence and convergence.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/deconstruct, selection, sequencing, stakes (DSSS)](<Evergreens/deconstruct, selection, sequencing, stakes (DSSS).md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/double diamond model (design)](<Evergreens/double diamond model (design).md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Evergreens/low floor, high ceiling](<Evergreens/low floor, high ceiling.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [February 10th, 2021](<February 10th, 2021.md>)
- [Brandon Toner](<Brandon Toner.md>)

- [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 11th, 2021](<February 11th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [Brandon Toner](<Brandon Toner.md>)

- [*]([Brandon Toner](<Brandon Toner.md>))

## [February 12th, 2021](<February 12th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [@]([Brandon Toner](<Brandon Toner.md>))

## [February 13th, 2021](<February 13th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 14th, 2021](<February 14th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [ ] Look into Twitter handles. [*]([Brandon Toner](<Brandon Toner.md>))

## [February 15th, 2021](<February 15th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [ ] Complete review of TODOs in the graph, prioritizing the date-tagged ones. [February 15th, 2021](<February 15th, 2021.md>) [*]([Brandon Toner](<Brandon Toner.md>))

- [ ] Review [Beau Hann](<Beau Hann.md>)'s [zettelkasten](<zettelkasten.md>) [conventions](<conventions.md>). [*]([Brandon Toner](<Brandon Toner.md>))

## [February 16th, 2021](<February 16th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- Chat with [Brandon Toner](<Brandon Toner.md>)

## [February 17th, 2021](<February 17th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [x] Review [Roaman Agora](https://roamresearch.com/#/app/The-Roaman-Agora) for opportunities to improve RC design and [onboarding](<onboarding.md>). [*]([Brandon Toner](<Brandon Toner.md>))

## [February 18th, 2021](<February 18th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [ ] Write about managing [chaos](<chaos.md>) in a [collaborative graph](<collaborative graph.md>). [*][Brandon Toner](<Brandon Toner.md>)

## [February 19th, 2021](<February 19th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 1st, 2021](<February 1st, 2021.md>)
- [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 20th, 2021](<February 20th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [@Brandon]([Brandon Toner](<Brandon Toner.md>))

## [February 21st, 2021](<February 21st, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 22nd, 2021](<February 22nd, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 23rd, 2021](<February 23rd, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 24th, 2021](<February 24th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 25th, 2021](<February 25th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 26th, 2021](<February 26th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- Been thinking hard on this one lately given conversation with [Brandon Toner](<Brandon Toner.md>)

## [February 28th, 2021](<February 28th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 2nd, 2021](<February 2nd, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- "[Charles Farr](<Charles Farr.md>), [Larissa de Lima](<Larissa de Lima.md>), & [Brandon Toner](<Brandon Toner.md>)

- [Brandon Toner](<Brandon Toner.md>)

- [Charles Farr](<Charles Farr.md>), [Larissa de Lima](<Larissa de Lima.md>), & [Brandon Toner](<Brandon Toner.md>)

- [Brandon Toner](<Brandon Toner.md>)

## [February 3rd, 2021](<February 3rd, 2021.md>)
- [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 4th, 2021](<February 4th, 2021.md>)
- Different from announcement, which is controlled in [your]([Brandon Toner](<Brandon Toner.md>))

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 5th, 2021](<February 5th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- Chat with [Brandon Toner](<Brandon Toner.md>)

## [February 6th, 2021](<February 6th, 2021.md>)
- what on earth am I doing here? [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 7th, 2021](<February 7th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [February 8th, 2021](<February 8th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [Brandon Toner](<Brandon Toner.md>):

## [February 9th, 2021](<February 9th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [If old memories still upset you, write them down carefully and completely.](<If old memories still upset you, write them down carefully and completely..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [If you have to choose, be the one who does things, instead of the one who is seen to do things.](<If you have to choose, be the one who does things, instead of the one who is seen to do things..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Imagine who you could be, and then aim single-mindedly at that.](<Imagine who you could be, and then aim single-mindedly at that..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [January 25th, 2021](<January 25th, 2021.md>)
- Jump right in! [I'll]([Brandon Toner](<Brandon Toner.md>))

- Jump right in! [I'll]([Brandon Toner](<Brandon Toner.md>))

- 14:00-19:06 — [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

1. [Brandon Toner](<Brandon Toner.md>)

1. "[~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

1. "[~](<~.md>) [Brandon Toner](<Brandon Toner.md>)

6. "[~](<~.md>) [Brandon Toner](<Brandon Toner.md>)

- [Brandon Toner](<Brandon Toner.md>)

- [~](<~.md>) [Brandon Toner](<Brandon Toner.md>)

- [~](<~.md>) [Brandon Toner](<Brandon Toner.md>)

- [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

## [January 26th, 2021](<January 26th, 2021.md>)
- 10:00 — 11:00 played around a bit. [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- **[Participants](<Participants.md>):** [Jason Griffing](<Jason Griffing.md>), [Beau Hann](<Beau Hann.md>), [Adam Bartley](<Adam Bartley.md>), [David Bieber](<David Bieber.md>), [Norman Chella](<Norman Chella.md>), [Lindsey Johnston](<Lindsey Johnston.md>), [Brandon Toner](<Brandon Toner.md>),

- [Brandon Toner](<Brandon Toner.md>)

- "I've landed on " [Brandon Toner](<Brandon Toner.md>)

## [January 27th, 2021](<January 27th, 2021.md>)
- From `[@](<@.md>)[Brandon Toner](<Brandon Toner.md>)`

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- "It's a small thing but could we could shift some of the tags and default template test to make them easier to select? Changing `[not-populated](<not-populated.md>)` to `[not_populated](<not_populated.md>)` makes it possible to select the text with a single double click in order to delete it when you're ready. [Same thing should extend to any of the 'dummy' text inside templates that's meant to be deleted.](#[My Daily Notes](<My Daily Notes.md>) [Your Name](<Your Name.md>) {{word-count}}) Thoughts? [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)"

- "Is there discussion/dialogue convention. I see here [⬆️](((HjQ5425kF))), a convention to get your attention. Where are the standards here. I thought I saw it before you did some of the restructuring. [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)"

- "What are the ideas for creating a dashboard for seeing how people are getting your attention. You can't efficiently query at this point using our conventions. If I was to create a query `{{[query](<query.md>): {and: [@](<@.md>) [Mark Robertson](<Mark Robertson.md>)}}}` I will not get my own `taps`, but instead get the ones that I have created on my DNP. The easy way, but don't know how stable is to add a `{not:}` for each member, but that seems to be an update nightmare.  [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)"

- "One thing that has been clear with all the multiplayer graphs I have worked with, is that zooming in on the bullet/area you are working on CAN be helpful to allow [Roam](<Roam.md>) to more efficiently sync changes AND it eases content moving right before your eyes. - since we will in effect be on different pages, instead of on one. [~](<~.md>) [Brandon Toner](<Brandon Toner.md>)"

- "There is also a disconnect in my mind, because of the nature of this graph's purpose, between what is `[Feedback](<Feedback.md>)` and what is a `[Question](<Question.md>)`. Is there something more specific for the feedback, as in elements that are built and we have feedback on. And question would be pushing the frontiers as well as potential suggestions. [~](<~.md>) [Brandon Toner](<Brandon Toner.md>)"

- "One thing that has been clear with all the multiplayer graphs I have worked with, is that zooming in on the bullet/area you are working on CAN be helpful to allow [Roam](<Roam.md>) to more efficiently sync changes AND it eases content moving right before your eyes. - since we will in effect be on different pages, instead of on one. [~](<~.md>) [Brandon Toner](<Brandon Toner.md>)"

- "That helps. Explorers will always find the path, and show the way for others. And for builders, sometimes let others determine that paths they would take, before establishing predefined funnels. This is a general observation about building spaces for people. For example, many European nations (particularly Scandinavia) do not build paths through parks and open spaces UNTIL people determine what way they would want to go. [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)"

- "[~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

- Loving some of these tags and their css tweaks. "It's a small thing but could we could shift some of the tags and default template test to make them easier to select? Changing `[not-populated](<not-populated.md>)` to `[not_populated](<not_populated.md>)` makes it possible to select the text with a single double click in order to delete it when you're ready. [Same thing should extend to any of the 'dummy' text inside templates that's meant to be deleted.](#[My Daily Notes](<My Daily Notes.md>) [Your Name](<Your Name.md>) {{word-count}}) Thoughts? [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)"

- It's a small thing but could we could shift some of the tags and default template test to make them easier to select? Changing `[not-populated](<not-populated.md>)` to `[not_populated](<not_populated.md>)` makes it possible to select the text with a single double click in order to delete it when you're ready. [Same thing should extend to any of the 'dummy' text inside templates that's meant to be deleted.](#[My Daily Notes](<My Daily Notes.md>) [Your Name](<Your Name.md>) {{word-count}}) Thoughts? [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

- [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

- 12:30 - EDN, JSON, and Markdown [backup](<backup.md>) is up and running with ownership being transferred to [Brandon Toner](<Brandon Toner.md>)

- Is there discussion/dialogue convention. I see here [⬆️](((HjQ5425kF))), a convention to get your attention. Where are the standards here. I thought I saw it before you did some of the restructuring. [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

- That helps. Explorers will always find the path, and show the way for others. And for builders, sometimes let others determine that paths they would take, before establishing predefined funnels. This is a general observation about building spaces for people. For example, many European nations (particularly Scandinavia) do not build paths through parks and open spaces UNTIL people determine what way they would want to go. [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

- One thing that has been clear with all the multiplayer graphs I have worked with, is that zooming in on the bullet/area you are working on CAN be helpful to allow [Roam](<Roam.md>) to more efficiently sync changes AND it eases content moving right before your eyes. - since we will in effect be on different pages, instead of on one. [~](<~.md>) [Brandon Toner](<Brandon Toner.md>)

- You maybe right with your comment here: "Is this captured by this tip? [~[[Mark Robertson](<~[[Mark Robertson.md>)]] "Click on any bullet to "zoom in" for a more focused perspective (reducing the noise, and focusing on your section) - this also helps with stability if there are a lot of us writing simultaneously."" . Though I know that Zooming is under-the-hood different, from collapse. Basically collapsing is a change of state, not of page. Where if you zoom in, you are actually on another URL. [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

- What are the ideas for creating a dashboard for seeing how people are getting your attention. You can't efficiently query at this point using our conventions. If I was to create a query `{{[query](<query.md>): {and: [@](<@.md>) [Mark Robertson](<Mark Robertson.md>)}}}` I will not get my own `taps`, but instead get the ones that I have created on my DNP. The easy way, but don't know how stable is to add a `{not:}` for each member, but that seems to be an update nightmare.  [~](<~.md>)[Brandon Toner](<Brandon Toner.md>)

- There is also a disconnect in my mind, because of the nature of this graph's purpose, between what is `[Feedback](<Feedback.md>)` and what is a `[Question](<Question.md>)`. Is there something more specific for the feedback, as in elements that are built and we have feedback on. And question would be pushing the frontiers as well as potential suggestions. [~](<~.md>) [Brandon Toner](<Brandon Toner.md>)

## [January 28th, 2021](<January 28th, 2021.md>)
- "12:10 — **Graph restored after crash lasted for >12 hours**. EDN format used. No known data loss. - [Brandon Toner](<Brandon Toner.md>)"

- 12:10 — **Graph restored after crash lasted for >12 hours**. EDN format used. No known data loss. - [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- Connected briefly with [Brandon Toner](<Brandon Toner.md>)

- I invited [Brandon Toner](<Brandon Toner.md>)

- [@[[Kyle Stratis](<@[[Kyle Stratis.md>)]] related to your comment [here](((bIl7_WLyg))), [Brandon Toner](<Brandon Toner.md>)

## [January 29th, 2021](<January 29th, 2021.md>)
Thoughts? - [Brandon Toner](<Brandon Toner.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

Thoughts? - [Brandon Toner](<Brandon Toner.md>)"

Thoughts? - [Brandon Toner](<Brandon Toner.md>)"

## [January 30th, 2021](<January 30th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- "According to the [definition](((o2aZIL3oU))) of [seedlings](<seedlings.md>) and the [context](((8zuNrwoHM))) on how it’s used from [Brandon Toner](<Brandon Toner.md>),

- "According to the [definition](((o2aZIL3oU))) of [seedlings](<seedlings.md>) and the [context](((8zuNrwoHM))) on how it’s used from [Brandon Toner](<Brandon Toner.md>),

- According to the [definition](((o2aZIL3oU))) of [seedlings](<seedlings.md>) and the [context](((8zuNrwoHM))) on how it’s used from [Brandon Toner](<Brandon Toner.md>),

## [January 31st, 2021](<January 31st, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- [ ] Change convention from Comments to Conversation (in alignment with [[[Roam Book Club](<[[Roam Book Club.md>) III]]) [February 1st, 2021](<February 1st, 2021.md>) [Brandon Toner](<Brandon Toner.md>)

## [Lectures/Maps of Meaning - JBP (lecture series)](<Lectures/Maps of Meaning - JBP (lecture series).md>)
- [Brandon Toner](<Brandon Toner.md>)

## [Maintain your connections with people.](<Maintain your connections with people..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Make at least one thing better every single place you go.](<Make at least one thing better every single place you go..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Make friends with people who want the best for you.](<Make friends with people who want the best for you..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [March 12th, 2021](<March 12th, 2021.md>)
- #[Graph Change Log](<Graph Change Log.md>)
        - **[Brandon Toner](<Brandon Toner.md>):**

## [March 13th, 2021](<March 13th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 14th, 2021](<March 14th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 1st, 2021](<March 1st, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

- As [Brandon Toner](<Brandon Toner.md>)

- [Clubhouse](<Clubhouse.md>) chat with [Brandon Toner](<Brandon Toner.md>)

## [March 22nd, 2021](<March 22nd, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 28th, 2021](<March 28th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 2nd, 2021](<March 2nd, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 3rd, 2021](<March 3rd, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 4th, 2021](<March 4th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 5th, 2021](<March 5th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 6th, 2021](<March 6th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 8th, 2021](<March 8th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [March 9th, 2021](<March 9th, 2021.md>)
- #[Main Feed](<Main Feed.md>) ((A place to showcase graph highlights throughout the day)) 
        - **[Brandon Toner](<Brandon Toner.md>):**

- #[My Daily Notes](<My Daily Notes.md>) [Brandon Toner](<Brandon Toner.md>)

## [Multiplayer Roam is more fun than single-player Roam.](<Multiplayer Roam is more fun than single-player Roam..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Nothing well done is insignificant.](<Nothing well done is insignificant..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Notice that opportunity lurks where responsibility has been abdicated.](<Notice that opportunity lurks where responsibility has been abdicated..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Pay attention.](<Pay attention..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Pet a cat when you encounter one on the street.](<Pet a cat when you encounter one on the street..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Plan and work diligently to maintain the romance in your relationships.](<Plan and work diligently to maintain the romance in your relationships..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Projects/Outline structure for Roam Collective Reading Group (RBC4)](<Projects/Outline structure for Roam Collective Reading Group (RBC4).md>)
- [Brandon Toner](<Brandon Toner.md>)

## [Projects/Publish a [Roam Collaboration Guide](<Roam Collaboration Guide.md>)](<Projects/Publish a [Roam Collaboration Guide](<Roam Collaboration Guide.md>).md>)
- **[Project Lead](<Project Lead.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Projects/Submit Grant Application to [Urbit](<Urbit.md>) for RC](<Projects/Submit Grant Application to [Urbit](<Urbit.md>) for RC.md>)
- [Brandon Toner](<Brandon Toner.md>)

## [Proverbs/stand on the shoulders of giants](<Proverbs/stand on the shoulders of giants.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Pursue what is meaningful (not what is expedient).](<Pursue what is meaningful (not what is expedient)..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Questions/How could an "agile" approach to collaboration be implemented in Roam Collective?](<Questions/How could an "agile" approach to collaboration be implemented in Roam Collective?.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Questions/What, why, how: Conventions to define the relationships in the graph?](<Questions/What, why, how: Conventions to define the relationships in the graph?.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Read something written by someone great.](<Read something written by someone great..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Remember that what you do not yet know is more important than what you already know.](<Remember that what you do not yet know is more important than what you already know..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Seedlings/The use of prepositional linkages empowers the mapping of dependencies and relationships in a graph database.](<Seedlings/The use of prepositional linkages empowers the mapping of dependencies and relationships in a graph database..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Seedlings/just-in-time vs just-in-case](<Seedlings/just-in-time vs just-in-case.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Seedlings/knowledge graphs should be populated opportunistically to optimize for flow state writing.](<Seedlings/knowledge graphs should be populated opportunistically to optimize for flow state writing..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):**  [Brandon Toner](<Brandon Toner.md>)

## [Seedlings/mutually exclusive, collectively exhaustive (MECE)](<Seedlings/mutually exclusive, collectively exhaustive (MECE).md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>),

## [Set your house in perfect order before you criticize the world.](<Set your house in perfect order before you criticize the world..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Stand up straight with your shoulders back.](<Stand up straight with your shoulders back..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Tell the truth, or at least don't lie.](<Tell the truth, or at least don't lie..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Treat yourself as if you were someone that you are responsible for helping.](<Treat yourself as if you were someone that you are responsible for helping..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Treat yourself like someone you are responsible for helping.](<Treat yourself like someone you are responsible for helping..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Try to make one room in your house as beautiful as possible.](<Try to make one room in your house as beautiful as possible..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Woah](<Woah.md>)
- [Brandon Toner](<Brandon Toner.md>)

## [Work as hard as you possibly can on at least one thing and see what happens.](<Work as hard as you possibly can on at least one thing and see what happens..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [Write a letter to the government if you see something that needs fixing -- and propose a solution.](<Write a letter to the government if you see something that needs fixing -- and propose a solution..md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [[project management](<[project management.md>) in Roam](<[project management](<project management.md>) in Roam.md>)
- I can elaborate more on this. - [Brandon Toner](<Brandon Toner.md>)

## [complex page names](<complex page names.md>)
- `[Brandon Toner](<Brandon Toner.md>)`

## [falling between the cracks](<falling between the cracks.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [graph editors](<graph editors.md>)
- Message [Brandon Toner](<Brandon Toner.md>)

## [grist for the mill](<grist for the mill.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

## [prepositional linkages](<prepositional linkages.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>)

- **[Author](<Author.md>):** [Brandon Toner](<Brandon Toner.md>)

