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
            - tests
        - tests
            - ```javascript

:q [:find (pull ?e [[:block/string]
                    [:block/uid]
                    [:edit/time]
                    [:edit/seen-by]]) 
    :where 
    [?f :node/title "Quote"]  
     [?e :block/refs ?f]
    ]


:q [:find (pull ?f [[:block/string]
                    [:block/uid]
                    [:edit/time]
                    [:edit/seen-by]]) 
    :where 
    [?f :block/uid "a8H7Z1PC5"]  
    ]


:q [:find ?members ?uid
 	:where 
    	[?b :user/display-name ?members]
		[?b :user/uid ?uid]
		[?b :db/id] ?id]]

:q [:find (pull ?user [
                    [:user/display-name]
                    ]) 
    :where 
      [?f :block/uid "a8H7Z1PC5"]  
      [?f :edit/user ?user]]

      
      
queryText = `[:find (pull ?e [[:block/string][:block/uid]])
     		            :in $ ?pagetitle
     		            :where
     		                [?f :node/title ?pagetitle]
     		                [?e :block/refs ?f]]`;

          result = window.roamAlphaAPI.q(queryText, "Quotes");
          console.log(result);
```
            - :q [:find (pull ?user [:user/display-name]) .
    :where 
      [?f :block/uid "a8H7Z1PC5"]  
      [?f :edit/user ?user]]
            - :q [:find ?members 
 	:where 
    	[?b :graph/settings ?members]
		]
            - :q [:find ?members ?uid ?email
 	:where 
    	[?b :user/display-name ?members]
		[?b :user/uid ?uid]
		[?b :user/email ?email]]
        - noti test
            - stable roam42
                - [Roam42](http://roam42.com/)
                    - {{[roam/js](<roam/js.md>)}}
                        - ```javascript

// DISABLE FEATURES 
// Remove two forward slashes from in front of name 
// of feature to DISABLE it 
// Everything is enabled by default 
window.disabledFeatures = [ 
  // 'quickReference', 
    // 'turnDown', 
    // 'dateProcessing', 
    // 'lookupUI', 
     'livePreview', 
     'dailyNote', 
    // 'templatePoc', 
    // 'jumpToDate', 
    // 'jumpNav', 
];


var s = document.createElement('script');
	s.type = "text/javascript";
  	s.src =  "https://roam42.glitch.me/main.js";
  	s.async = true;
document.body.appendChild(s);
```
                    - Settings
                        - [42Setting](<42Setting.md>) DailyNotePopup off
                        - [42Setting](<42Setting.md>) LivePreview off
                    - Shortcuts
                        - Natural language date processing -`ALT+SHIFT+D`
            - remove icon
                - {{[roam/js](<roam/js.md>)}}
                    - ```javascript


var elem = document.getElementById("notification-center-button");
  elem.parentNode.removeChild(elem);
var element2 = document.getElementById("notification-center-flex-space");
	element.parentNode.removeChild(element2);```
            - [remote reload](https://github.com/austinbirch/roam-cljs-example)
                - {{[roam/js](<roam/js.md>)}}
                    - ```javascript
var s = document.createElement("script");
s.src = "http://127.0.0.1:8081/internal_notifications_masonry.js";
s.id = "roamnotifications";
s.type = "text/javascript";
document.getElementsByTagName("head")[0].appendChild(s);```
            - local noti
                - {{[roam/js](<roam/js.md>)}}
                    - ```javascript
// this heavily cribs from roam42 and random-page-plugin.js
(()=>{
  notificationCenter = {};
  notificationCenter.tippy = {};
  loadNotificationCenterIcon = async ()=>  {
    // this is the page to watch for notifications
    // TODO find a better way of doing this...
      var pageToWatch = 'roam/css';

      var mySleep = m => new Promise(r => setTimeout(r, m));
      //Loop to check if roam-topbar has been loaded yet... if not, sleep for a bit to wait for it
      for (let y = 1; y < 20; y++) {
          if (document.getElementsByClassName("rm-topbar") != null &&
              document.getElementsByClassName("roam-body-main") != null &&
              document.getElementById("right-sidebar") != null) {
              if (document.getElementsByClassName("rm-topbar").length > 0 &&
                  document.getElementsByClassName("roam-body-main").length > 0) { break; }
          }
          await mySleep(100);
      }

      // Sleep for an extra little bit to load later than other icons to help with
      // ordering left to right (200 = 3rd)
      await mySleep(200);

      function loadCSS(){
          var styles = `
              .unread-notifications.bp3-icon-notifications::before {
                  color: red; }
          `

          var styleSheet = document.createElement("style")
          styleSheet.type = "text/css"
          styleSheet.innerText = styles
          document.head.appendChild(styleSheet)
      }

      function convertTimestamp(time){
        const options = {
        	// weekday: 'long',
        	year: 'numeric',
        	month: 'numeric',
        	day: 'numeric',
        	hour: 'numeric',
          minute: 'numeric'};

        const dateTimeFormat = new Intl.DateTimeFormat('en-us', options);
        return dateTimeFormat.format(time);
      }

      // load the notifications when the button is clicked
      displayMenu = async ()=>{
          const db = location.hash.split('/')[2];
          let menu = '';
          menu += `<div class="notification-center bp3-popover-content">
                    <div class="bp3-menu">
                      <header>
                        <div class="notification-header"><strong class="bp3-icon-notifications bp3-intent" tabindex="0" role="button"> Notifications</strong></div>
                        <div class="bp3-button-group bp3-fill">
                          <a class="bp3-button bp3-icon-inbox bp3-intent bp3-active" tabindex="0" role="button">Mentions</a>
                          <a class="bp3-button bp3-icon-git-new-branch bp3-intent bp3-disabled" tabindex="0" role="button">Refs</a>
                        </div>
                      </header>
                      <div class="message-container">`;
          // query for all references to your pageToWatch
          query = `[:find (pull ?e [[:block/string][:block/uid][:edit/time]])
     		            :in $ ?pagetitle
     		            :where
     		                [?f :node/title ?pagetitle]
     		                [?e :block/refs ?f]]`;

          result = window.roamAlphaAPI.q(query, pageToWatch);
          watchPageUIDQuery = `[:find (pull ?e [:block/uid]) .
                 		            :in $ ?pagetitle
                 		            :where
                 		                [?e :node/title ?pagetitle]]`;

          // get the url for your pageToWatch
          var pageToWatchUID = window.roamAlphaAPI.q(watchPageUIDQuery, pageToWatch).uid;
          var pageToWatchURL = `https://roamresearch.com/#/app/${db}/page/${pageToWatchUID}`
          console.log(result);

          for (i = 0; i < result.length; i++) {
              if (!result[i][0].string.includes('{{[query](<query.md>):')){ //skip {{queries}}
                var blockUID = result[i][0].uid
                var displayNameQuery = `[:find (pull ?user [:user/display-name]) .
            		            :in $ ?block
            		            :where
            		                [?f :block/uid ?block]
            		                [?f :edit/user ?user]]`;
                var displayName = window.roamAlphaAPI.q(displayNameQuery, blockUID)['display-name'];
                console.log(displayName);

                var editTime = convertTimestamp(result[i][0].time)
                var blockURL = `https://roamresearch.com/#/app/${db}/page/${blockUID}`
                // menu += `<div class="flex-v-box rm-menu-item">
                //             <ul>
                //               <li class="rm-search-list-item">
                //                 <a href="${blockURL}" class="bp3-menu-item bp3-popover-dismiss">
                //                   ${result[i][0].string}
                //                 </a>
                //               </li>
                //             </ul>
                //           </div>`;
                menu += `<div class="dialog-box bp3-menu-item bp3-popover-dismiss">
                            <div class="metadata">
                              <div class="contents">
                                <div class="left"><strong>${displayName}</strong></div>
                                <div class="right">${editTime}</div>
                              </div>
                            </div>
                            <div class="contents main-content"><p>${result[i][0].string}</p></div>
                          </div>`;
          }}
          menu += '</div></div></div>'
      return menu;
      }

      //Add css for notificaion icon
      loadCSS();

      createMenu = async ()=>{}
      //Add button (thanks Tyler Wince!)
      var nameToUse = 'notification-center';
      //Find icons to use at: https://blueprintjs.com/docs/[icons](<icons.md>)
      var bpIconName = 'notifications';

      var checkForButton = document.getElementById(nameToUse + '-icon');
      if (!checkForButton) {
          // add overarching div
          var mainButton = document.createElement('span');
            mainButton.id = nameToUse + '-button';
            mainButton.classList.add('bp3-popover-wrapper');
          var spanTwo = document.createElement('span');
            spanTwo.classList.add('bp3-popover-target');
            mainButton.appendChild(spanTwo);
          var mainIcon = document.createElement('span');
            mainIcon.id = nameToUse + '-icon';
            //check if there are existing notificaitons
            queryText = `[:find (pull ?e [[:block/string][:block/uid]])
        								:in $ ?pagetitle
        								:where
        									[?f :node/title ?pagetitle]
        									[?e :block/refs ?f]]`;
        		let notiResults= window.roamAlphaAPI.q(queryText, pageToWatch);
            if (notiResults.length > 0){
                mainIcon.classList.add('unread-notifications',
                                      'bp3-icon-' + bpIconName,
                                      'bp3-button',
                                      'bp3-minimal',
                                      'bp3-small');
            }else {
                mainIcon.classList.add('bp3-icon-' + bpIconName,
                                      'bp3-button',
                                      'bp3-minimal',
                                      'bp3-small');
            }
          spanTwo.appendChild(mainIcon);
          var roamTopbar = document.getElementsByClassName("rm-topbar");

          var nextIconButton = roamTopbar[0].lastElementChild;
          var flexDiv = document.createElement('div');
            flexDiv.id = nameToUse + '-flex';
            flexDiv.className = 'rm-topbar__spacer-sm';
          nextIconButton.insertAdjacentElement('afterend', mainButton);
          mainButton.insertAdjacentElement('afterend', flexDiv);

          // mainButton.addEventListener('click', displayMenu);

          notificationCenter.tippy = tippy(`#${nameToUse}-button`, {
            allowHTML: true,
            interactive: true,
            interactiveBorder: 5,
            arrow: false,
            trigger: 'click',
            position: 'auto',
            onShow(instance) {
              setTimeout(async ()=>{
                var elem = document.getElementById(instance.popper.id).firstElementChild
                if(window.innerWidth < elem.getBoundingClientRect().right ){
                  elem.style.left = '-' + Number(elem.style.width.replace('px','')) + 'px';
                }
                instance.setContent( await displayMenu() )
              },50)
            },
            onMount(instance) {
                      setTimeout(async ()=>{
                        // ${nameToUse}
                          var bck = document.querySelector(`[notification-center-button](<notification-center-button.md>) + div .tippy-box`);
                          console.log(bck);
                          bck.style.width="400px";
                		  bck.classList.add('bp3-popover');

                          instance.setContent( await displayMenu() ); //force content in for sizing
                      },50)
            },
          });

          tippy(`#${nameToUse}-button`, {
            content: `<div class="bp3-popover-content">Notifications</div>`,
            allowHTML: true,
            arrow: false,
            theme: 'light-border',
          });
      }
  }
})();
loadNotificationCenterIcon();
```
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
            - "[Conversation](<Conversation.md>) "
            - notifications
                - {{[mentions](<mentions.md>): [notification](<notification.md>)}}
            - {{[embed](<embed.md>): ((((kXB8zvMec))))}}

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

