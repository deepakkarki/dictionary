# Dictionary
This is an humble effort to create a simple, clean, easy to use and to the point android dictionary application.
The current solutions are bloated, hard to use or just full of advertisements. This application aims to be a community supported open-source dictionary app for android.

###Features 
* Word lookup should give me meaning, pronunciation, sample sentances, synonyms and antonyms (if applicable).
* Drop down suggestion during word search search.
* A way to 'favourite' words.
* "shake" to get a new word.
* Should be available offline.

###How to start
* First collect the complete database of words ( + thesaurus?) into JSON format
  * This can be done either by parsing websites or using API services. Parsing may be sticky, better to go for API and locally download. 
  * In case of API - first look at Apple's dictionary (+ thesaurus + wikipedia), then look at stuff like merriam, google and Wordnik API as well.
  * If API does not give all the data, just go and parse the web pages.
* Next, after having the JSON database, create a REST based API for all the words. Use Python's Flask. This REST API is useful for the online version of the dictionary app. 
* Now start coding the android app, initially use the online REST API to get all the details.
* Finally offer a offline dictionary - probably have to store on a local sqlite-db. 
* Keep coming up with updates in terms of extra features and big fixes. None of the features should be a *bloat*.
