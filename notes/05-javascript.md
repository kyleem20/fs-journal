# JavaScript

class notes:
https://github.com/BoiseCodeWorks/LateFall21-JsDayOne

https://github.com/BoiseCodeWorks/late-fall21-js-day2

reading notes:
A function is a subprogram designed to perform a particular task.
Function definitions are hoisted — expressions are not.
Functions are executed when they are called. This is known as invoking a function.
Values can be passed into functions and used within the function. The name of the value is called a parameter. The actual value itself is called an argument.
Functions always return a value. In JavaScript, if no return value is specified, the function will return undefined by default.
Functions are objects.


Parameters are used when defining a function, they are the names created in the function definition. In fact, during a function definition, we can pass in up to 255 parameters! Parameters are separated by commas in the ().
Arguments, on the other hand, are the values the function receives from each parameter when the function is executed (invoked).

Function Declaration: defines a named function. To create a function declaration you use the function keyword followed by the name of the function. When using function declarations, the function definition is hoisted, thus allowing the function to be used before it is defined
Function Expression: Function Expressions defines a named or anonymous function. An anonymous function is a function that has no name. Function Expressions are not hoisted, and therefore cannot be used before they are defined
Arrow Function Expression: shorter syntax for writing function expressions. Arrow functions do not create their own this value.



file name: app.js
script src="app.js">/script>

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
