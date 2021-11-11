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





11/9
All you need to do is figure out which character is most frequent for each position. 

let data = `eedadn
drvtee
eandsr
raavrd
atevrs
tsrnev
sdttsa
rasrtv
nssdts
ntnada
svetve
tesnvt
vntsnd
vrdear
dvrsen
enarar`.split('\n')

//input String[]
function repeaterCode(arr){
let out = ''
for(let col = 0; col < arr[0].length; col++){

  let seen = {}
  let greatest = ''
  let greatestCount = 0
  for(let row =0; row < arr.length; row++ ){
    const char = arr[row][col]
    seen[char] = seen[char] || 0
    seen[char]++
    if(seen[char]> greatestCount){
      greatestCount = seen[char]
      greatest = char
    }
  }
}
return out
}
//output String



11/10
https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/intermediate-algorithm-scripting/diff-two-arrays

Compare two arrays and return a new array with any items only found in one of the two given arrays, but not both. In other words, return the symmetric difference of the two arrays.

function diffArray(arr1, arr2) {
  var newArr = [];

  function onlyInFirst(first, second) {
    // Looping through an array to find elements that don't exist in another array
    for (var i = 0; i < first.length; i++) {
      if (second.indexOf(first[i]) === -1) {
        // Pushing the elements unique to first to newArr
        newArr.push(first[i]);
      }
    }
  }

  onlyInFirst(arr1, arr2);
  onlyInFirst(arr2, arr1);

  return newArr;
}

diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5]);

--

function diffArray(arr1, arr2) {
  return arr1
    .concat(arr2)
    .filter(item => !arr1.includes(item) || !arr2.includes(item));
}

diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5]);

--

function diffArray(arr1, arr2) {
  return [...diff(arr1, arr2), ...diff(arr2, arr1)];

  function diff(a, b) {
    return a.filter(item => b.indexOf(item) === -1);
  }
}
diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5]);
--

function diffArray(arr1, arr2) {
  var newArr = [];
  arr1.forEach(elem=>{
    if(!arr2.includes(elem)){
      newArr.push(elem)
    }
  })
  arr2.forEach(elem => {
    of(!arr1.includes(elem)){
      newArr.push(elem)
    }
  })
  return newArr;
}
diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5]);

------
You will be provided with an initial array (the first argument in the destroyer function), followed by one or more arguments. Remove all elements from the initial array that are of the same value as these arguments.

function destroyer(arr) {
  let valsToRemove = Object.values(arguments).slice(1);

  for (let i = 0; i < arr.length; i++) {
    for (let j = 0; j < valsToRemove.length; j++) {
      if (arr[i] === valsToRemove[j]) {
        delete arr[i];
      }
    }
  }
  return arr.filter(item => item !== null);
}

--

function destroyer(arr) {
  var valsToRemove = Array.from(arguments).slice(1);
  return arr.filter(function(val) {
    return !valsToRemove.includes(val);
  });
}

--

function destroyer(arr, ...valsToRemove) {
  return arr.filter(elem => !valsToRemove.includes(elem));
}


----------

11/11

Whiteboard Challenges

Jeep="Jeep", trail="__##_###___##_#"


function trailScanner(Jeep, trail){
let JeepSize = Jeep.length
let BigRock = 0
for(let i=0, i < trail.length; i++){
let char = trail[i]
if(char == "#"){
  BigRock++
  if(JeepSize <= BigRock){
    return False
  }
} else {
  BigRock = 0
}

}

return true
}

----------




