- ### What is this?
    - Custom Components are blocks created out of clojurescript functions that will update in realtime as you modify the code 
    - It's only a toy right now but has huge potential
    - First you must enable **Custom Components** in your user settings
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FRoam-Collective%2FH29QielpBU.png?alt=media&token=9990a5e9-6547-46e0-af17-f28d22c8313d)
- # Examples
    - Simple Bar Graph Component
        - {{[roam/render](<../roam/render.md>): ((Jhcqnk3e7))}}
            - test block```clojure

(defn chart [_]
  [:html 
 [:head 
  [:style ".chart-body {background-color:transparent !important;}.chart div {\nfont: 10px sans-serif;\nbackground-color: steelblue;\ntext-align: right;\npadding: 3px;\nmargin: 1px;\ncolor: tan;\n}\n.chart div:nth-child(1) {\nwidth: 40px;\n}\n.chart div:nth-child(2) {\nwidth: 80px;\n}\n.chart div:nth-child(3) {\nwidth: 150px;\n}\n.chart div:nth-child(4) {\nwidth: 160px;\n}\n.chart div:nth-child(5) {\nwidth: 230px;\n}\n.chart div:nth-child(6) {\nwidth: 420px;\n}
   "]
  ] 
 [:body {:class "chart-body"}
  [:div {:class "chart"} 
   [:div "4"] 
   [:div "8"] 
   [:div "15"] 
   [:div "16"] 
   [:div "23"] 
   [:div "42"]
   ]]
 ]
  )
```
    - Sample [hypothes.is](https://hypothes.is/) card
        - {{[roam/render](<../roam/render.md>): ((xr-heMOua))}}
            - ```clojure

(defn hypo [_]
  	[:html [:head [:style ".hypo-body {background-color:transparent !important;}.annotation-card {font-family: \"Helvetica\", sans-serif;font-size: 13px;border: 1px solid rgb(236, 236, 236);list-style: none;padding: 13px;margin-bottom: 10px;box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.4);background: rgb(255, 255, 255);overflow-wrap: break-word;max-width: 400px;}.annotation-card:hover {box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.45);}.annotation-card:hover .annotation-card__quote {border-left: rgb(247, 145, 88) 3px solid;color:black !important;}.annotation-card:hover .annotation-card__timestamp{color: rgb(122, 122, 122) !important;}.annotation-card:hover .annotation-card__username{color: rgb(122, 122, 122) !important;}.annotation-card:hover .annotation-card__text{color: rgb(122, 122, 122) !important;}.annotation-card__header {color: rgb(166, 166, 166) !important;margin-bottom: 15px;-ms-flex-align: baseline;align-items: baseline;}.annotation-card__username-timestamp {display: -ms-flexbox;display: flex;-ms-flex-direction: row;flex-direction: row;-ms-flex-pack: justify;justify-content: space-between}.annotation-card__username {color: rgb(166, 166, 166) !important;font-style: italic;font-weight: 200}.annotation-card__timestamp {font-size: 11px;line-height: 12px;font-weight: 400;letter-spacing: .2px;color: rgb(166, 166, 166) !important;}.annotation-card__text {line-height: normal;overflow-wrap: break-word;color:rgb(166, 166, 166) !important;font-weight: 400;}.annotation-card__text h1,.annotation-card__text h2,.annotation-card__text h3,.annotation-card__text h4,.annotation-card__text h5,.annotation-card__text h6,.annotation-card__text p,.annotation-card__text ol,.annotation-card__text ul,.annotation-card__text img,.annotation-card__text pre,.annotation-card__text blockquote {margin: .618em 0}.annotation-card__text h1,.annotation-card__text h2,.annotation-card__text h3,.annotation-card__text h4,.annotation-card__text h5,.annotation-card__text h6 {font-family: \"Helvetica Neue\", Helvetica, Arial, \"Lucida Grande\", sans-serif}.annotation-card__text h1 {font-size: 2.618em;font-weight: bold;margin: .2327em 0}.annotation-card__text h2 {font-size: 1.991em;font-weight: bold;margin: .309em 0}.annotation-card__text h3 {font-size: 1.991em;margin: .309em 0}.annotation-card__text h4 {font-size: 1.618em;margin: .3803em 0}.annotation-card__text h5 {font-size: 1.231em;margin: .4944em 0}.annotation-card__text h6 {font-size: 1.231em;margin: .4944em 0}.annotation-card__text ol,.annotation-card__text ul {list-style-position: inside;padding-left: 0}.annotation-card__text ol ol,.annotation-card__text ol ul,.annotation-card__text ul ol,.annotation-card__text ul ul {padding-left: 1em}.annotation-card__text ol {list-style-type: decimal}.annotation-card__text ul {list-style-type: disc}.annotation-card__text ol ul,.annotation-card__text ul ul {list-style-type: circle}.annotation-card__text li {margin-bottom: .291em}.annotation-card__text li,.annotation-card__text p {line-height: 1.3}.annotation-card__text a {text-decoration: underline}.annotation-card__text img {display: block;max-width: 100%}.annotation-card__text blockquote {font-size: 13px;line-height: 15px;font-weight: 400;border-left: 3px solid rgb(219, 219, 219);color: rgb(166, 166, 166) !important;font-family: sans-serif;font-size: 12px;font-style: italic;letter-spacing: .1px;padding: 0 1em;margin: 1em 0}.annotation-card__text blockquote p,.annotation-card__text blockquote ol,.annotation-card__text blockquote ul,.annotation-card__text blockquote img,.annotation-card__text blockquote pre,.annotation-card__text blockquote blockquote {margin: .7063em 0}.annotation-card__text blockquote p,.annotation-card__text blockquote li {line-height: 1.5}.annotation-card__text code {font-family: Open Sans Mono, Menlo, DejaVu Sans Mono, monospace;font-size: .875em;color: rgb(0, 0, 0)}.annotation-card__text pre code {padding: 10px;display: block;background-color: rgb(242, 242, 242);border-radius: 2px}.annotation-card__quote {padding: 0 10px;overflow-wrap: break-word;color: rgb(77, 77, 77) !important;font-weight: bold;font-family: sans-serif;font-size: 14px;font-style: italic;letter-spacing: .1px;border-left: 3px solid rgb(219, 219, 219);margin-bottom: 10px;margin-left: 0;margin-right: 0}.annotation-card__tags {display: -ms-flexbox;display: flex;-ms-flex-direction: row;flex-direction: row;-ms-flex-wrap: wrap;flex-wrap: wrap}.annotation-card__tag {text-decoration: none;border: 1px solid rgb(219, 219, 219);border-radius: 2px;padding: 0 5px 2px;color: rgb(122, 122, 122);background: rgb(242, 242, 242);margin: 0 5px 5px 0;font-size: 11px;cursor: pointer;white-space: nowrap;overflow: hidden;text-overflow: ellipsis}.annotation-card__footer {display: -ms-flexbox;display: flex;-ms-flex-direction: row;flex-direction: row;-ms-flex-pack: end;justify-content: flex-end;-ms-flex-align: baseline;align-items: baseline}.annotation-card__footer-link {margin-left: 15px;color: rgb(166, 166, 166);height: 16px;width: 16px;float:left}.annotation-card__incontext-link {height: 14px;width: 14px;padding-top: 1px}.annotation-card__incontext-link:visited {color: rgb(122, 122, 122)}.svg-icon {transform: translateX(0)}svg {-webkit-tap-highlight-color: rgba(255, 255, 255, 0)}a,a:active,a:focus,a:hover {text-decoration: none}ul,ol,li {border: 0;list-style: none;margin: 0;padding: 0}*,*:after,*:before {box-sizing: border-box}a {background-color: transparent}html,body{background-color: var(--page-color, rgb(255, 255, 255)) !important;}"]] [:body {:class "hypo-body"} [:li{:class "annotation-card"}[:div{:class "annotation-card__header"}[:div{:class "annotation-card__username-timestamp"}[:a{:title "username",:href "$user_url",:target "_blank",:class "annotation-card__username"}"$username"] [:a{:title "date",:href "$url",:target "_blank",:class "annotation-card__timestamp"}"$date"]]] [:blockquote{:title "Annotation quote",:class "annotation-card__quote"}"$highlight"] [:div{:class "annotation-card__text"}[:p "$annotation"]] [:footer{:class "annotation-card__footer"}[:a{:href "$url",:rel "nofollow noopener",:target "_blank",:title "Visit annotation in context"}[:svg{:xmlns "http://www.w3.org/2000/svg",:class "svg-icon annotation-card__footer-link annotation-card__incontext-link",:height "11",:viewbox "0 0 11 11",:width "11"}[:path{:d "M7.586 2H4V0h5.997A1.002 1.002 0 0111 1.003V7H9V3.414l-7.293 7.293L.293 9.293 7.586 2z",:fill "currentColor",:fill-rule "evenodd"}]]]]]]]
  )```

# Backlinks
## [February 4th, 2021](<February 4th, 2021.md>)
- [@[[Zsolt Viczián](<../@[[Zsolt Viczián.md>)]] has put together several smartblock templates that will run a datalog query and display it in a nice way. It's great work and an exceptionally good article but in my opinion actually pollutes the graph with `:hiccup` blocks. The better way would probably be to use [roam/render](<../roam/render.md>)

## [roam/render](<roam/render.md>)
- {{[roam/render](<../roam/render.md>):

- {{[roam/render](<../roam/render.md>):

