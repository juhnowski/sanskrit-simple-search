# 14-05-2017
* Store word frequency usage to localStorage. It was implemented by word_frequency.js which is converted from text data file by java program. Once it prepared it may be used till time when frequency data will be changed. Java converter is in https://github.com/juhnowski/FreqWordList url.
* add server.js - this is node.js simple http server for testing. LocalStorage is working only with domains.When I opened fetching.html as file, localStorage was inaccessible.

* run local http server:
  * install node.js https://nodejs.org/en/
  * install http-server https://www.npmjs.com/package/http-server via npm:   npm install http-server -g
  * run server: node server.js
  * test url in CHROME: http://localhost:8080/fetching.html and don't forget switch on CORS plugin

* TODO:
  * word list ordering by desc word.frequency. Now it's display in parentheses before word name.
  * changes  test.filter = "roman";  test.noLit = "off";  test.transLit="slp1"; which are now hardcoded.

# 13-05-2017
Add fetching.html - yet another iteration of search UI component

Please pay attention:
1)It will work correct from http://www.sanskrit-lexicon.uni-koeln.de site.
2)For correct work in local browser it's needed to install Google chrome plugin:
https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi/related?hl=en-US

Previously we talk about getting data from server in JSON format, but I stay on parsing incoming html, becouse:
1) to keep the backward compatibility
2) not to spend time and forces on changes in a backend and then support two version of server responses: html and json
