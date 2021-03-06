







# The Story of Javascript

- Q: Why do we need to know Javascript?
















- ECMAScript is the official language name

- Currently the world's most popular programming language (but not the best!).

- Way to make web pages dynamic.

- Created in 10 days at Netscape by Brendan Eich in 1995.

- Scripting language for the browser, alternative to Java.

- Has great parts and terrible parts, but we're stuck with it because of backwards-compatibility requirements of the web.

- Slowly evolving (ES5 and ES6).

- Client-side vs. Server-side programming.

- Document Object Model (DOM) is the API the browser provides to Javascript for modifying a web page.

- Without Javascript, need to load a fully new page every time we want anything to change on the page => Slow and unresponsive. Javascript lets us respond to user input, or update the page, immediately.







# Our First Dynamic Page






- Demo:
  Create an html file with head script tag in that write's "Hello, World" to the page.










- Demo:
  Change script to write out the current date.










- Inline Javascript with the "script" tag.










- Demo:
  Extract the javascript out to an external script and load it.
  => Loading external scripts with "src".
  => Loading remote scripts with a URL.








- Exercise:
  Add a second external script that write's your name to the page.













# REPLs

- JS console in Chrome and Firefox
- Shortcuts for console and reload
- repl.it













# Numbers







- Demo: numbers
  - very similar to Ruby










- Demo: numbers and arithmetic
  - * + - / %
  - very similar to Ruby










- Q: What is 1/2 in Ruby?
- Q: What is 1/2 in Javascript?
  => All numbers are floats in JS!









- Remember: All numbers are floats, unlike Ruby








# Strings






- Demo strings
  => Very similar to Ruby













- "", '', \n, \"












- Concatenation
  => with + instead of interpolation with #{}












- Getting the length with '.length'
  => Not with size or count











- Getting a character with `charAt`









- Exercise:
  Create a string "Hello, [Your Name]!" by concatenating 3 strings.











- Exercise:
  Compute the length of the string you just created.










- Remember: concatenation, length, charAt










# Variables

- Demo: Variables










- End statements with a semi-colon ';'

- Declare variables with 'var' before use.










- Short-hand for declare and initialize at the same time.











- Naming convention: lowerCamelCase variable names.












- Example:
  Create two variables containing numbers and a third contains their sum. Use only 3 lines of code.










- Exercise:
  - Assign a variable as your first name.
  - Assign a variable as your last name.
  - Assign a variable as your full name by combining the above with a space between.















- Key points: Must declare variables with 'var' before using. Semi-colons separate statements.











# Debugging





- Demo: console.log









- Demo: debugger










- Comments









- Exercise:
    Change "Our First Dynamic Page" to write the following message to the console:
      "Hello, Mitch! In case you forgot, the result of 3 x 4 is 12."

    Use variables for your name, a, b, and result.











- Exercise:
    Change your script to write this message to the console AND the document.













- Exercise:
    Add a comment to the top of the script describing what it does.











- Remember: console.log is like "puts", # => //








# Built-Ins






- Demo in console:
  - alert => display a message
  - confirm => true if ok, false if cancel
  - prompt => string or null if cancel









- null
  => like Ruby's nil => nothing










- Exercise:
  Change your script message to write to the document, console.log AND create an alert.









- Exercise:
  Change your script to prompt the user for their name and then alert "Hello, [name]!"








#Logic

- Demo in console
  => Similar to Ruby
  => true, false, > < == != <= >=, &&, ||, !










- Q: What is result of ("abc" > "def")









- Q: What is ("2" == 2)?











- Remember: looser equality












# Conditionals

- Demo: if, if-else, if-else-if

```js
if (condition) {
  // ...
} else if (otherCondition) {
  // ...
} else {
  // ...
}
```











- "If" is a statement, not an expression:

```js
// Not valid JS
var answer = if (a) { 2; } else { 3; }
```












- Exercise: Build a Safe

  Change our script to prompt a user for the password to our safe.
  If the password is correct, create an alert message with a success message and reveal the safe's secret. Otherwise alert a failure message.

  E.g.:
  "Welcome to the safe! What is the password?"
  [enter correct password]
  "Access Granted! The secret is 'I like pie'"
  [enter incorrect password]
  "Access Denied!"












- Exercise: A safe with confirmation

  Change your safe so that it asks the user if they wants to enter the safe first.

  E.g.:

  "Welcome to super-safe! Do you want to enter?"
  "OK. Goodbye, then."










- Remember: (), {}, "else if". statement vs expression










# Loops

- Demo: while loop

```js
while (condition) {
  // Body
}
```

  => +=
  => Like ruby, but with () and {}












- Example:
  Log the numbers from 0 to 100 to the console.















- Exercise: Log the evens
  Log the EVEN numbers from 0 to 100 to the console.













- Exercise: Bottles of beer

  Implement "bottles of beer rhyme"

  e.g.
  "100 bottles of beer on the wall"
  "100 bottles of beer"
  "Take one down, pass it around, 99 bottles of beer on the wall"









- Demo: for loop

```js
  for (var i=5; i < 10; i += 1) {
    console.log(i);
  }

  for (initialize; condition; increment) {
    // ...
  }
```

  => Convenience of having initialization, condition and increment together, because often use it.






- Exercise: Bottle of beer with "for"

  Implement "bottles of beer rhyme" with "for"

  e.g.
  "100 bottles of beer on the wall"
  "100 bottles of beer"
  "Take one down, pass it around, 99 bottles of beer on the wall"












- Exiting early with "break"











- Example:

  Determine the first number divisible by 3,4, and 5 using a "while" loop and "break".
















- Exercise: Sum to 99

  Use a "for" loop to determine the sum of the numbers from 0 to 99














- Exercise: Safe with 3 strikes

  Make a script the prompts users for a password.
  If they get the password correct, alert a success message.
  If they get the password wrong, let them retry 3 times before denying them access.

  You should use a "for" loop, and "break".

  Scenario 1:
    "What is the password?"
    [enters wrong password]
    "What is the password?"
    [enters wrong password]
    "What is the password?"
    [enters wrong password]
    "Three tries, you're out. Access Denied!"

  Scenario 2:
    "What is the password?"
    [enters correct password]
    "Access granted!"






- Converting a string to a number with parseInt and parseFloat.
- Converting a number to string with .toString()













- Optional Exercise: Number guessing game

  Demo: Creating a random number from 0 - 100
  Prompt users to guess a number between 0 - 100 until they guess right.
  Alert the user on each guess whether it is greater or less than their guess.
  Alert when they get it right.









# Arrays

- Demo: Arrays
  => Like ruby arrays












- push, pop, shift, unshift, []











- length
  => (no size or count methods)













- Exercise: Array of numbers
  Make an array containing the digits from 0 to 100.










- Example: Looping through an array










- Exercise: Loop through words
  - Create an array of strings: ["apple", "dog", "computer", "cup"]
  - Loop through the array and log to the console:
    "[Word] has [length] characters."













- split, join














- Exercise: Count words
  Write a script that prompts for a sentence, and alerts how many words are in that sentence.













- Exercise: String of digits
  Make a string containing all the numbers from 0-99.













# Functions

- Demo: Functions, function expressions, calling functions













- Returning values.
  => Must have explicit return.










- Example: greeter
  Write a function that accepts a name, and returns the string "Hello, [name]!"










- Example: reverseArray
  Write a function "reverse" that accepts an array, and returns an array with the items in reverse order.











- Exercise: double
  write a function "double" to double a number.












- Exercise: doubleArray
  write a function that accepts an array of numbers and returns a array of those numbers doubled.
  Use your "double" function above.











- First-class functions
    => First class citizens in JS.
       Can store in variables, pass as parameters, and return => Lots of power.
    => More similar to blocks / lamdas in Ruby than methods.








- Passing functions as parameters to other functions.








- Example: Multi-printer

  Write a function to print the length of a sentence using different printers.

  e.g. printWords("Hello there!", console.log);
  Using console.log, alert, document.write












- Exercise: map

  Write a function "map" which accepts an array and a function "transform", and returns an array where each item is the result of calling "transform" on the item of the original array.

  e.g.
  var increment = function (number) { return number + 1; }
  map([1, 2, 3], increment); => [2, 3, 4];











- Exercise: doubleArray with map

  Re-write doubleArray using your "map" function.











- Demo: Passing anonymous functions as parameters.
  => Using "map" and "printWords"











- Functions as parameters in the wild.
  => Used in lots of APIs that we will see.
  => Examples on underscorejs.org website.









- setInterval, setTimeout

- Example: counter with setInterval












- Ending an interval with "clearInterval"













- Exercise: Blast-off

  Build a blast-off countdown using setInterval.
  10 9 8 7 6 5 4 3 2 1 Blast Off!









- Exercise: force accept

  Write a script that continues to ask the user to donate money to your website, every second until they click "OK". When they click OK, thank them and stop prompting.








# Objects

- Demo: Object literal
  => Like a Ruby hash.
  => Strings are always keys.






- Setting, getting, adding keys with '.'








- Demo: Building a car
  Build a "car" object, and add/change properties.






- Q: What happens when you access a property that doesn't exist?










- Exercise: Me Object

  Create an object "me" containing you name, age, and occupation.








- Demo: nested objects
  Add a "car" object to "me" object










- Accessing and setting nested properties.









- Q: What if you want to have a key with a space in it?










- Demo: [] notation
  => for keys with spaces.
  => for keys from expressions.










- Exercise: Word lengths

  Write a function that takes a sentence, and returns an object of all the words and their lengths.

  wordLengths("Hello world"); => { "Hello": 5, "world": 5 }












- Exercise: User age (without "if")

  Write a function "userAge" that takes a user's name, and returns their age. If the user is not found, return "undefined". Don't use any "if" statements.

  Here are the age's of your users:
  joe is 32, john is 40, shirley is 28, and joan is 54












- deleting properties with "delete"














- Looping over properties (for-in loop)













- Example: Count properties
    Write a function that computes the number of properties an object has.











- Exercise:
    "console" is an object, figure out what properties it has.

















- Exercise: Clone
  Write a function "clone", which takes an object and returns a clone of it.











- Adding functions to objects (like methods).











- Example:
    Adding "drive" function to "car" object that says "vrrooooomm!".
    Calling "drive".






- This is what we've seen when calling console.log!















- Exercise: Stopping car
    Add a stop function to your car that logs "screeetch!" to the console.










# Documentation

- MDN docs for Array, String, ... (explain what prototype means)









# Topics we didn't cover

  - functions on objects
  - "this" keyword inside functions.
  - Closures
  - Creating objects with "new"











# Homework

- In certified.in
- Preview Jukebox exercise







