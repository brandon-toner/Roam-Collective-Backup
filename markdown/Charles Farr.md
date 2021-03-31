- Tags:: #People #Members #Moderators
    - About me::
        - Twitter:: [@CharlesSimsFarr](https://twitter.com/CharlesSimsFarr)
        - Website:: [Foundation.al — personal blog](https://thefoundation.al)
        - Location:: Chicago, IL
        - Time Zone:: Central Time (GMT –6:00)
    - Status::
        - {{or:🟢Online | 😴 Offline | 🟠Away}}
- :hiccup [:hr]
- # Personal Artifacts
    - SmartBlocks
        - #42SmartBlock CFarr — DNP
            - #[[My Daily Notes]] [[Charles Farr]] [°]([[csf]]) {{word-count}} — {{or:🟢Online | 😴 Offline | 🟠Away}}
                - #Scratchpad #not-populated
                - #Conversation #not-populated
                - #Bookmarks #not-populated
            - ---
    - Custom JavaScript
        - Indexing code
            - {{[[roam/js]]}}
                - ```javascript
/*
Query to pull block references of all block-level tags
  Examples include: #Q, #Syn, #Notion
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

  // blockTag = '#Syn'; // changed to be an input
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
        - #min-con {{[[query]]: {and: [[csf]] [[Q]] {not: {or: }}  }}}
    - Follow Ups
        - #min-title {{[[query]]: {and: [[csf]] [[Follow Up]] {not: {or: }}  }}}
    - Bookmarks
        - #min-con {{[[query]]: {and: [[csf]] [[Bookmarks]] {not: {or: [[not-populated]] }}  }}}
    - Todos
        - #min-con {{[[query]]: {and: [[Charles Farr]] [[TODO]] {not: {or: [[query]] }}  }}}
    - Daily Notes
        - #min-con {{[[query]]: {and: [[Charles Farr]] [[csf]] {not: {or: [[query]] [[42SmartBlock]] }}  }}}
    - Query on keywords
        - {{[[query]]: {and: [[Charles Farr]] [[taxonomy]] {not: {or: [[query]] }}  }}}
- # Personal Shortcuts
    - [[datalog experimentation]]
    - [@ mentions for me]([[@[[Charles Farr]]]])
