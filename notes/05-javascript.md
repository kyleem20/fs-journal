# JavaScript

file name: app.js
<!-- <script src="app.js"></script> -->

**Primitive Types**

*Value Types* (don't retain relationship)
-
let number = -.2 <-any number
let string = "words"
let char = "c" <- string of 1 character in js
let boolean = true or false <- one or the other

let notDefined = undefined <- you never assigned it
let noValue = null <- you know there is no value in there, put in on purpose as a value of nothing
-
*Reference Types* (retain relationship)
-
 Array store data by their position or INDEX
let array = ["a", "b", "c"]
console.log("access array data", array[1])

Objects store their data by KEY/PROPERTY and VALUE ( key : value )
let object = {a: "a", b: "b", c: "c"} or {a: "a", b: 2, c: false}
console.log("access object data", object["b], object.b)
-

Declaration vs Assignment
Declaration is when it is initially declared
Assignment is when it is in a new piece of code stated later on, new value is declared


++sum pre-operative
sum++ post-operative
% remainder of following number in to the variable

*Interpolate*
let interpolate = `this inserts into a specific spot ${"Welcome Name", welcomeName}
  the back ticks and $ creates the interpolate

*Switch*
let switchValue = 2

switch(switchValue){
  case 0:
    do this
  break;
  case 1:
    do this instead
  break;
  default: 
    if nothing else is true, do this instead
  break;
}

*Debugger*
Allows you to run through your code step by step in sources

Parameters:


Arguments:
