13-05-2017
Add fetching.html - yet another iteration of search UI component

Please pay attention:
1)It will work correct from http://www.sanskrit-lexicon.uni-koeln.de site.
2)For correct work in local browser it's needed to install Google chrome plugin:
https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi/related?hl=en-US

Previously we talk about getting data from server in JSON format, but I stay on parsing incoming html, becouse:
1) to keep the backward compatibility
2) not to spend time and forces on changes in a backend and then support two version of server responses: html and json
