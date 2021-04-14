- #[My Daily Notes](<My Daily Notes.md>) [Peter Rosso](<Peter Rosso.md>) {{word-count}} [*]([ptr](<ptr.md>))   {{or:🚫 Offline | 🟡 On & Off | 🟠Away | 🟢Online}}
    - [Inbox](<Inbox.md>) 
        - [ ] Update Query Display Options adding hover option
            - ```css
/* MINIMIZE QUERIES v2 by Jeff Harris
A feature of Roam Mosaic https://github.com/roam-mosaic/theme-boilerplate
  Add any of the following tags to your query (in the same block). They can be used in combination to customize what information is hidden
    #.q--q = hides the query
    #.q--title = hides the page title of the reference
    #.q--mentions = hides the contextual reference information (breadcrumbs) 
    #.q--bg = hides the background of each individual query result
    #.q--compact = removes extra space between each query result
    #.q--hover = shows title and mentions on hover of an individual query result
    #.q--all = hides everything with one tag, rendering the query nearly invisible
inspired by Matt Goldenberg 
*/
:root {
 --rm-linked-reference__backgound-color_1: [ebf1f5](<ebf1f5.md>);
}
.q--q .rm-query-title {
  display: none;
}
.q--title .rm-mentions .rm-ref-page-view .rm-title-arrow-wrapper {
  display: none;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
}
.q--mentions .rm-zoom {
  display: none;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
}
.q--mentions .rm-reference-item {
  padding: 0;
}
.q--bg .rm-reference-item {
  background: none;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
}
.q--compact .rm-reference-item {
  margin-left: -12px;
  margin-top: 3px;
  padding: 0;
}
.q--all .rm-query-title {
  display: none;
}
.q--all .rm-zoom {
  display: none;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
}
.q--all .rm-reference-main {
  padding-top: 0;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
}
.q--all .rm-block-input {
  padding-right: 0;
}
.q--all .rm-reference-item {
  background: none;
  margin: 0;
  margin-left: -12px;
  padding: 0;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
}
.q--all > div > div.roam-block {
  padding-top: 0;
}
.q--all .rm-mentions .rm-ref-page-view {
  margin: 0;
}
.q--all .rm-mentions .rm-ref-page-view .rm-title-arrow-wrapper {
  display: none;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
}
.q--all .rm-query {
  border: none;
}
.q--all .rm-query div[style*='margin-left: 12px;'] {
  margin-left: 0 !important;
}
.q--all .rm-query span[style='margin-left: 9px; font-size: 0.9em;'] {
  display: none;
}
.q--hover .rm-ref-page-view:hover .rm-zoom {
  display: flex;
}
.q--hover .rm-ref-page-view:hover .rm-reference-item {
  background: var(--rm-linked-reference__backgound-color_1);
}
.q--hover.q--all .rm-mentions .rm-ref-page-view:hover .rm-title-arrow-wrapper,
.q--hover.q--title .rm-mentions .rm-ref-page-view:hover .rm-title-arrow-wrapper {
  display: flex;
}```
    - #[Scratchpad](<Scratchpad.md>) [not-populated](<not-populated.md>)
    - [Conversation](<Conversation.md>) [not-populated](<not-populated.md>)
- ---
