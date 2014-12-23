{% include JB/setup %}

This is my first encounter with Java 8's lambdas. To use a lambda I created a functional interface. Conceptually, a functional interface has exactly one abstract method.

I then created a Test class that uses an anonymous class as well as a lambda expression to achieve the same result (printing out the function invocation).

The resulting output will be:

Function invoked using Anonymous class

Function invoked using Lambda expression
Back in the eighties I used to be a big fan of the IQ-Kwis, a quiz on Belgian television (http://nl.wikipedia.org/wiki/De_IQ-Kwis). The contestants had to answer knowledge questions and at the end of the show solve a word puzzle. Because these days the whole world seems to be doing AngularJS I wanted to familiarize myself with Angular by starting a little project implementing this word puzzle.

But while doing so I thought it would be nice to store puzzles' high scores as well and thought of exploring some cloud technology and use mongodb, express, rest and nodejs to implement the backend. I also thought it would be nice to have the final app be a mobile app and earn big money from it and retire. But that is just a side goal. My main goal is to relive the eighties and learn something on the side.


Something about the word puzzle...

The final round was the blackboard containing letters in a random order. Each team had to make a word as long as possible by shifting the letters. This was a variation on the sliding puzzle with 24 cubes of which 4 are blank. The longest possible word consisted of 20 letters.

The slide puzzle is a puzzle on a plate of 4 times 4 fields. In the most common variant are 15 fields a number, the numbers 1 to 15. A field is empty. Still can be pushed a figure to the empty field , which replace the empty field so shifts, hence the name puzzle.

http://en.wikipedia.org/wiki/Sliding_puzzle
