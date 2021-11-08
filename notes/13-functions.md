# Functions

Morning Warm Up notes:
Week 2 Day 2
let myObject = {
  item: 'fridge',
  color: 'white',
  height: 3,
  width: 2,
  working: true,
}
let description = myObject.item + ' is ' + myObject.height + ' feet by ' + myObject.width + ' feet'

console.log('My', description)

let bang = {
  color: 'red',
  shape: 'cylinder',
  sugar: false,
  caffeineMg: 300,
  ingredients: ['Taurine', 'BCAA', 'Caffeine', 'Red dye 3'],
  manufacturer: {
    name: 'VPX',
    location: '123 Main St',
  }
}

// Access every property: This can of bang is (color), and is in a (shape) container, it is (sugar free, has sugar), it also has (caffeineMG) mg of caffeine, the main ingredients are (list of ingredients), and it was made by (manufacturer name), at (manufacturer location)

let message = `This can of bang is ${bang.color}, and is in a ${bang.shape} container, it is ${bang.sugar ? 'has sugar' : 'is sugar free'}, it also has ${bang.caffeineMg} mg of caffeine, the main ingredients are ${bang.ingredients.join(' ')}, and it was made by ${bang.manufacturer.name}, at ${bang.manufacturer.location} `


if (bang.sugar) {
  'has sugar'
} else {
  'is sugar free'
}
console.log(message)
----
11/4
Given three numbers to represent the length of each side of a triangle, determine if the three numbers can actually make a triangle or not.
EX: 10, 20, 29 --> true
EX: 10, 20, 31 --> false
EX: 31, 10, 20 --> false
Option 1:
function isTriangle(num1, num2, num3){
    return (num1 < (num2 + num3) && num2 < (num1 + num3)&& num3 <(num2 + num1))
}
Option 2:
function isTriangleArray(...angles){
    let sorted = angles.sort((a,b) => a-b)
    console.log(sorted)
    return sorted[2] < sorted[1] + sorted[0]
}
isTriangleArray(10,20,29)
Option 3:
function isMaybeTriangle(a,b,c){
    const large = Math.max(...arguments)
    return large < (a+ b+ c) - large
}
