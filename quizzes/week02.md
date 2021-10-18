# Intro to JavaScript

**1.** Which keywords are used to declare a variable in JavaScript?
<!-- enter your answer in the space below -->
```
var, let, const
```
**2.** What is the definition of a function?
<!-- enter your answer in the space below -->
```
a way to perform particular tasks
```
**3.** What are the `SOLID` principles?
<!-- enter your answer in the space below -->
```
S — Single responsibility,
O — Open closed,
L — Liskov substitution,
I — Interface segregation,
D — Dependency Inversion
```
**4.** Given this array: 
```js
let fruit = ['apple', 'banana', 'pineapple',  'orange', 'strawberry']
``` 
What index is the pineapple's current position? How do you know?
<!-- enter your answer in the space below -->
```
[2], the locations start at 0 then increase by 1 after
```
**5.** With these two objects: 
```js
let you = { name:"You", hair: true, friends: [] }
let them = { name:"Them", hair: false, friends: [] }
```
how would you .push the `them` object into the `you` object's array of friends?
<!-- enter your answer in the space below -->
```
them.concat(you)
or
them.push(you)
```

**6.** Give an example of a JavaScript `Conditional`:
<!-- enter your answer in the space below -->
```
( ? ), ( : )
```
**7.** In the `for loop` below, what is the name of the piece belongs inside the empty "______" space? What would you put here to increase `i` by one on every iteration?
```js
for ( let i = 0; i < arr.length; _______ ) {
  //...
```
<!-- enter your answer in the space below -->

```
Indicator, i++
```
**8.** What does the `DOM` acronym stand for? Which file is first accessed to render the `DOM`?
<!-- enter your answer in the space below -->
```
Document Object Model; the document is first accessed
```

**9.** What are the `9` ECMAScript types as defined by MDN?
<!-- enter your answer in the space below -->
```
Boolean type, Null type, Undefined type, Number type, BigInt type, String type, Symbol type, Primitive Values, Objects
```
**10.** When it comes to functions or methods, what is the difference between a `parameter` and an `argument`?
<!-- enter your answer in the space below -->
```
Parameters are names used to define and create a function Arguments are the values run through a function when it is run
```
**11.** What is the difference between a `primitive` value and a `reference` value?
<!-- enter your answer in the space below -->
```
Primitive: data that are stored on the stack. Reference: objects that are stored in the heap.
```