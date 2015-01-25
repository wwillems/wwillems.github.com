---
layout: post
title: "Angular exploration - Sliding puzzle"
description: "Sliding puzzle project"
category: angular
tags: [angular]
---
{% include JB/setup %}


Back in the eighties I used to be a big fan of the <a href="http://nl.wikipedia.org/wiki/De_IQ-Kwis">IQ-Kwis</a>, a quiz on Belgian television. The contestants had to answer knowledge questions and at the end of the show solve a word puzzle. Because of AngularJS gaining traction I wanted to familiarize myself with Angular by starting a little project (I decided to name the project "Swiped") implementing this word puzzle.

But while doing so I thought it would be nice to store puzzles' high scores as well and thought of exploring some cloud technology and use mongodb, express, rest and nodejs to implement the backend.

Something about the word puzzle...

The final round was the blackboard containing letters in a random order. Each team had to make a word as long as possible by shifting the letters. This was a variation on the sliding puzzle with 24 cubes of which 4 are blank. The longest possible word consisted of 20 letters.

The slide puzzle is a puzzle on a plate of 4 times 4 fields. In the most common variant the 15 fields are numbers, the numbers 1 to 15. One field is empty. A number can be pushed to the empty field which then replaces the empty field, hence the name puzzle.

<a href="http://en.wikipedia.org/wiki/Sliding_puzzle">Sliding puzzle (wikipedia)</a>

The backend as well as the frontend are deployed on Heroku. The working version can be found here:

<a href="http://swiped.herokuapp.com">Swiped on Heroku</a>

The screenshot below shows the playing field of a four by four sliding puzzle. At the bottom of the playing field the running time is shown. Once the puzzle is completed, i.e. the numbers are shown is the proper order and the empty tile is in the bottom right corner, the score can be uploaded by clicking the 'Upload score' button.

[TODO add screenshot]

The high score can be viewed by selecting the 'High scores' entry in the Swiped menu. It shows a list of high scores showing the user name, the date of the high score, the playing level and the time needed to complete the puzzle. The search box can be used to select a specific player's scores.

This is a sample list of high scores:

[TODO add screenshot]

To register a new player profile use the <a href="http://swiped.herokuapp.com/register.html">registration form</a>. 

This is the registration form in full color:
[TODO add new screenshot]
<img src="http://swiped.herokuapp.com/images/swiped-register.jpg">

This form is based on the MailChimp signup form as described in this great post on onehungrymind <a href="http://onehungrymind.com/build-mailchimp-signup-form-angularjs/">Build a MailChimp Signup Form with AngularJS</a>.

The code can be found on github. The frontend (AngularJS) project can be found <a href="https://github.com/wwillems/swiped.git">here</a>. Whereas the backend (rest/node js) project can be found <a href="https://github.com/wwillems/scoreapi.git">here</a>.
