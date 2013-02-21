SmarterThan
===========

Webelos Game for Flag Requirements taking queues from "Smarter than a Fifth Grader" from U.S. Network Television. 

Purpose
-------

My Webelos scouts had to review some citizenship requirements from their handbook. The den leader manual had some ideas to make this fun; one of which was this particular game. I liked the idea, but thought we needed a cool display for the questions so I created this. It's very simple and editing the questions is as simple as adding JSON to the questions.js script. 

Implementation
--------------

I wanted this to be fast and have no live internet connection necessary, so I developed it as a stand-alone handlebars/jquery app to run locally off the browser. As it turns out, some of the scouts didn't make it to the meeting and I wanted them to be able to catch up on their own, so I published it through Heroku as a Node/Express app serving static files. It gets the job done and since the whole thing is client side and the JSON is small, the game loads and runs rather quickly.

Invitation
----------

Please fork for your own purposes; you can use this quiz format for just about anything!

Todos
-----

* Add support for Mobile (using JQuery Mobile)
  * because swipe would be nice
  * because there's no arrow keys on a mobile platform's browser (well, at least not iOS)

* Add support for displaying answers
  * I think adding a down button handler would be sufficient
  * Need to add a field in the JSON for an answer to the q

* Add support for on-screen navigation
  * in the case that a user doesn't want to press the arrow keys
  * JQuery-Mobile has a nice demo in the swipe example

* Make categories more distinquishable
  * add hover support (won't work on mobile)
  * underline current selection?
  * also need to separate the categories in a more readable way

