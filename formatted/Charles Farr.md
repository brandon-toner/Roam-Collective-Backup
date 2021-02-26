- **[Tags](<Tags.md>):** [People](<People.md>) [Members](<Members.md>) [Moderators](<Moderators.md>)
    - **[About me](<About me.md>):**
        - **[Twitter](<Twitter.md>):** [@CharlesSimsFarr](https://twitter.com/CharlesSimsFarr)
        - **[Website](<Website.md>):** [Foundation.al — personal blog](https://thefoundation.al)
        - **[Location](<Location.md>):** Chicago, IL
        - **[Time Zone](<Time Zone.md>):** Central Time (GMT –6:00)
    - **[Status](<Status.md>):**
        - {{or:🟢Online | 😴 Offline | 🟠Away}}
- :hiccup [:hr]
- # Personal Artifacts
    - SmartBlocks
        - [42SmartBlock](<42SmartBlock.md>) CFarr — DNP
            - #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>) [°]([csf](<csf.md>)) {{word-count}} — "{{or:🟢Online | 😴 Offline | 🟠Away}}"
                - [Scratchpad](<Scratchpad.md>) [not-populated](<not-populated.md>)
                - [Conversation](<Conversation.md>) [not-populated](<not-populated.md>)
                - [Bookmarks](<Bookmarks.md>) [not-populated](<not-populated.md>)
            - ---
    - Custom JavaScript
        - Indexing code
            - {{[roam/js](<roam/js.md>)}}
                - ```javascript
/*
Query to pull block references of all block-level tags
  Examples include: [Q](<Q.md>), [Syn](<Syn.md>), [Notion](<Notion.md>)
*/

// Function
// Inputs:
  // blockTag
  // indexPageTitle
  // parent_uid (optional)
// Outputs: Writes relevant blocks to

function updateIndexPage(tag_to_index, index_page, index_parent_uid) {

  // Step 0
  // Creates a rule to find all ancestors of a given block

  let ancestorRule = `[
    [(ancestor ?child ?parent)
    [?parent :block/children ?child]]
    [(ancestor ?child ?ancestor)
    [?parent :block/children ?child]
    (ancestor ?parent ?ancestor)]
  ]`;

  // Step 1
  // Find all blocks containing the specified block-level tag
  // Inputs:
    // blockTag — a block-level tag to build index on
  // Outputs:

  // blockTag = '[Syn](<Syn.md>)'; // changed to be an input
  let blockTag = tag_to_index;

  let blockPull = window.roamAlphaAPI.q(`
      [:find (pull ?eid [*])
       :in $ ?block_tag
          :where
       		   [?eid :block/string ?block_string]
  		       [(clojure.string/includes? ?block_string ?block_tag)]
           ]`,blockTag);

  let blockRefsWTag = [];

  for (var block in blockPull) {
    let blockRefId = '((' + blockPull[block][0].uid + '))';
    blockRefsWTag.push(blockRefId);
  };

  // Step 2
  // Find all blocks already references on the current page_title
  // Inputs:
    // indexPageTitle — title of the page to build the index on
  // Outputs:

  // let indexPageTitle = 'Test Index Page'; //change to be an input
  let indexPageTitle = index_page;

  let indexPageBlocks = window.roamAlphaAPI.q(`
    [:find
      (pull ?block [*])
      :in $ % ?index_page_title
      :where
        [?index_eid :node/title ?index_page_title]
        (ancestor ?block ?index_eid)]`
    , ancestorRule, indexPageTitle);

  let representedBlockRefs = [];

  for (var indexBlock in indexPageBlocks) {
    // pull string of block into variable
    let refString = indexPageBlocks[indexBlock][0].string;
    console.log(refString);

    // split string into components
    let splitString = refString.split(' ');
    console.log(splitString);

    // iterate through split components and select block refs
    for (var strComp in splitString) {
      console.log(splitString[strComp]);
      if (splitString[strComp].includes
        && splitString[strComp].includes("))")) {
      representedBlockRefs.push(splitString[strComp]);
      };
    };
  };

  console.log(representedBlockRefs);

  // Step 3
  // Create subset of all blocks from Step 1 that are not in Step 2
  // Inputs:
  // Outputs:

  let unindexedBlocks = [];

  for (var blockId in blockRefsWTag) {
    console.log(blockRefsWTag[blockId]);
    if (!(representedBlockRefs.includes(blockRefsWTag[blockId]))) {
      unindexedBlocks.push(blockRefsWTag[blockId]);
    }
  }


  // Step 4
  // Output block references onto page_title
  // Inputs:
  // Outputs:

  let pageRefQuery = window.roamAlphaAPI.q(`
      [:find (pull ?eid [*])
       :in $ ?index_page_title
       :where
          [?eid :node/title ?index_page_title]
           ]`,indexPageTitle);

//  let parent_uid = pageRefQuery[0][0].uid;
  let parent_uid = index_parent_uid;

  for (var blockId in unindexedBlocks) {
    let order = -1;
    let block = unindexedBlocks[blockId];

    window.roamAlphaAPI.createBlock(
        {
          "location": {"parent-uid": parent_uid, "order": order},
          "block": {"string": block}
        }
      )
  };
};

window.updateIndexPage = updateIndexPage;
```
- # Personal Queries
    - Questions
        - [min-con](<min-con.md>) {{[query](<query.md>): {and: [csf](<csf.md>) [Q](<Q.md>) {not: {or: }}  }}}
    - Follow Ups
        - [min-title](<min-title.md>) {{[query](<query.md>): {and: [csf](<csf.md>) [Follow Up](<Follow Up.md>) {not: {or: }}  }}}
    - Bookmarks
        - [min-title](<min-title.md>) {{[query](<query.md>): {and: [csf](<csf.md>) [Bookmarks](<Bookmarks.md>) {not: {or: [not-populated](<not-populated.md>) }}  }}}
    - Todos
        - [min-con](<min-con.md>) {{[query](<query.md>): {and: [Charles Farr](<Charles Farr.md>) [TODO](<TODO.md>) {not: {or: [query](<query.md>) }}  }}}
    - Daily Notes
        - [min-con](<min-con.md>) {{[query](<query.md>): {and: [Charles Farr](<Charles Farr.md>) [csf](<csf.md>) {not: {or: [query](<query.md>) [42SmartBlock](<42SmartBlock.md>) }}  }}}
    - Query on keywords
        - {{[query](<query.md>): {and: [Charles Farr](<Charles Farr.md>) [taxonomy](<taxonomy.md>) {not: {or: [query](<query.md>) }}  }}}
- # Personal Shortcuts
    - [datalog experimentation](<datalog experimentation.md>)
    - [@ mentions for me]([@[[Charles Farr](<@[[Charles Farr.md>)]])

# Backlinks
## [Charles Farr](<Charles Farr.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- [min-con](<min-con.md>) {{[query](<query.md>): {and: [Charles Farr](<Charles Farr.md>)

- [min-con](<min-con.md>) {{[query](<query.md>): {and: [Charles Farr](<Charles Farr.md>)

- {{[query](<query.md>): {and: [Charles Farr](<Charles Farr.md>)

## [Evergreens/Evergreen notes should be concept-oriented](<Evergreens/Evergreen notes should be concept-oriented.md>)
- [Charles Farr](<Charles Farr.md>)

## [February 10th, 2021](<February 10th, 2021.md>)
- [Charles Farr](<Charles Farr.md>)

- "Some `[@[[Charles Farr](<@[[Charles Farr.md>)]]` mentions don't show up within my `[Charles Farr](<Charles Farr.md>)`

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- Some `[@[[Charles Farr](<@[[Charles Farr.md>)]]` mentions don't show up within my `[Charles Farr](<Charles Farr.md>)`

- [^[[Brandon Toner](<^[[Brandon Toner.md>)]] not entirely sure which ones are [missing](((N2piKtO8Z))) — weird thing is they all show up on the actual `[@[[Charles Farr](<@[[Charles Farr.md>)]]`, just not the `[Charles Farr](<Charles Farr.md>)`

## [February 11th, 2021](<February 11th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 12th, 2021](<February 12th, 2021.md>)
- **Brandon:** Exploration of the idea of [prepositional linkages](((yfs_C3Z9A)))
        - **[Charles Farr](<Charles Farr.md>):**

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 13th, 2021](<February 13th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- Contributor → `[Charles Farr](<Charles Farr.md>)`

- People would be represented by pages (e.g., `[Charles Farr](<Charles Farr.md>)`

## [February 14th, 2021](<February 14th, 2021.md>)
- Building "[Roaman Agora](<Roaman Agora.md>)" -- [Charles Farr](<Charles Farr.md>)

- Integrating [roam-inter](<roam-inter.md>) into [Roaman Agora](<Roaman Agora.md>) -- [Charles Farr](<Charles Farr.md>)

## [February 15th, 2021](<February 15th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 16th, 2021](<February 16th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 17th, 2021](<February 17th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 18th, 2021](<February 18th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 19th, 2021](<February 19th, 2021.md>)
- Incorporating [play](<play.md>) into your life [Interintellect](<Interintellect.md>) I+([Charles Farr](<Charles Farr.md>))

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- Each chat would be registered with a member page, e.g., `Chat/[Charles Farr](<Charles Farr.md>)`

- 09:58 | `Chat/[Charles Farr](<Charles Farr.md>):

## [February 1st, 2021](<February 1st, 2021.md>)
- Reflection on any of the [How To](<How To.md>) pages [Charles Farr](<Charles Farr.md>)

- From [Charles Farr](<Charles Farr.md>):

- "#[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- [Charles Farr](<Charles Farr.md>)

- #[FN](<FN.md>) "Establishing levels within [evergreen notes](<evergreen notes.md>) lowers the bar to creation and raises the bar for [maturity](<maturity.md>)." - [Charles Farr](<Charles Farr.md>)[

- "Reflection on any of the [How To](<How To.md>) pages [Charles Farr](<Charles Farr.md>)

- Regarding "Reflection on any of the [How To](<How To.md>) pages [Charles Farr](<Charles Farr.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 20th, 2021](<February 20th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 22nd, 2021](<February 22nd, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 23rd, 2021](<February 23rd, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 24th, 2021](<February 24th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 25th, 2021](<February 25th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 26th, 2021](<February 26th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 2nd, 2021](<February 2nd, 2021.md>)
- "[Charles Farr](<Charles Farr.md>),

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- [Charles Farr](<Charles Farr.md>),

## [February 3rd, 2021](<February 3rd, 2021.md>)
- Color directory (setup by [Charles Farr](<Charles Farr.md>))

- [Charles Farr](<Charles Farr.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- ""#[FN](<FN.md>) "Establishing levels within [evergreen notes](<evergreen notes.md>) lowers the bar to creation and raises the bar for [maturity](<maturity.md>)." - [Charles Farr](<Charles Farr.md>)[

- ""The [block referenced aspects](((Kq6jZZIYI))) of the zettelkasten note template proposed by [Charles Farr](<Charles Farr.md>)

## [February 4th, 2021](<February 4th, 2021.md>)
- **Larissa** I like this!
            - **[Charles Farr](<Charles Farr.md>):**

- **Matt V**: Yes
            - **[Charles Farr](<Charles Farr.md>):**

- **Brandon:** Ou! Cool idea. Totally. How do we get it set up? [~[[Peter Rosso](<~[[Peter Rosso.md>)]]
            - **[Charles Farr](<Charles Farr.md>):**

- **Matt V:** Honestly it doesn't look like any of the [query css](((KOuJf-Smr))) is doing anything...
            - **[Charles Farr](<Charles Farr.md>):**

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 5th, 2021](<February 5th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 6th, 2021](<February 6th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 7th, 2021](<February 7th, 2021.md>)
1. Last night I ([Charles]([Charles Farr](<Charles Farr.md>))

- "Last night I ([Charles]([Charles Farr](<Charles Farr.md>))

6. Thoughts on [this](((bUlmW8JmS)))? [*]([Charles Farr](<Charles Farr.md>))

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 8th, 2021](<February 8th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [February 9th, 2021](<February 9th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [January 25th, 2021](<January 25th, 2021.md>)
- Thoughts? [~](<~.md>) [Charles Farr](<Charles Farr.md>)

- [Charles Farr](<Charles Farr.md>)

- Maybe `[Resources](<Resources.md>)`? [~](<~.md>)[Charles Farr](<Charles Farr.md>)

- Thoughts on this? [~](<~.md>)[Charles Farr](<Charles Farr.md>),

- [~](<~.md>)[Charles Farr](<Charles Farr.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- "Maybe `[Resources](<Resources.md>)`? [~](<~.md>)[Charles Farr](<Charles Farr.md>)"

## [January 26th, 2021](<January 26th, 2021.md>)
- Made a few minor additions as I worked through open questions. [Charles Farr](<Charles Farr.md>)

- Thoughts on this? [~](<~.md>)[Charles Farr](<Charles Farr.md>)

- "Riffing while in transit..." [Charles Farr](<Charles Farr.md>)

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

- [Charles Farr](<Charles Farr.md>)

- "Thoughts on this? [~](<~.md>)[Charles Farr](<Charles Farr.md>)"

- "Added a [Resources Template](((gix1P4auD))) cc: [~](<~.md>)[Charles Farr](<Charles Farr.md>)"

- "[~](<~.md>)[Charles Farr](<Charles Farr.md>)

- "Thoughts on this? [~](<~.md>)[Charles Farr](<Charles Farr.md>),

- "Thoughts? [~](<~.md>) [Charles Farr](<Charles Farr.md>)"

## [January 28th, 2021](<January 28th, 2021.md>)
-  20:19 — Brief [Clubhouse](<Clubhouse.md>) conversation with [Akiff Premjee](<Akiff Premjee.md>), [Charles Farr](<Charles Farr.md>)

- " 20:19 — Brief [Clubhouse](<Clubhouse.md>) conversation with [Akiff Premjee](<Akiff Premjee.md>), [Charles Farr](<Charles Farr.md>)

- [Charles Farr](<Charles Farr.md>):

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [January 30th, 2021](<January 30th, 2021.md>)
- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [January 31st, 2021](<January 31st, 2021.md>)
- The [block referenced aspects](((Kq6jZZIYI))) of the zettelkasten note template proposed by [Charles Farr](<Charles Farr.md>)

- Love [Charle's]([Charles Farr](<Charles Farr.md>))

- #[My Daily Notes](<My Daily Notes.md>) [Charles Farr](<Charles Farr.md>)

## [Projects/Submit Grant Application to [Urbit](<Urbit.md>) for RC](<Projects/Submit Grant Application to [Urbit](<Urbit.md>) for RC.md>)
- **[Created by](<Created by.md>):** [Charles Farr](<Charles Farr.md>)

- **[Project Lead](<Project Lead.md>):** [Charles Farr](<Charles Farr.md>)

## [Questions/What, why, how: Conventions to define the relationships in the graph?](<Questions/What, why, how: Conventions to define the relationships in the graph?.md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>) (on behalf of [Charles Farr](<Charles Farr.md>))

- **[Author](<Author.md>):** [Charles Farr](<Charles Farr.md>)

## [Questions/When does chaos become insurmountable?](<Questions/When does chaos become insurmountable?.md>)
- **[Created by](<Created by.md>):** [Charles Farr](<Charles Farr.md>)

## [Seedlings/mutually exclusive, collectively exhaustive (MECE)](<Seedlings/mutually exclusive, collectively exhaustive (MECE).md>)
- **[Created by](<Created by.md>):** [Brandon Toner](<Brandon Toner.md>), from [Charles Farr](<Charles Farr.md>)'

## [Summary/of maturity of notes](<Summary/of maturity of notes.md>)
- "#[FN](<FN.md>) "Establishing levels within [evergreen notes](<evergreen notes.md>) lowers the bar to creation and raises the bar for [maturity](<maturity.md>)." - [Charles Farr](<Charles Farr.md>)[

- "The [block referenced aspects](((Kq6jZZIYI))) of the zettelkasten note template proposed by [Charles Farr](<Charles Farr.md>)

