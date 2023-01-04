# Financial Analysis

## Link to site

## Description / How it works

## Issues and Solutions

#### 1. Don't forget to use `= `to assign, and `==` or `===` in maths. 

#### 2. Calculation displaying too many decimal places. 
`.toFixed(x)` will round number to x decimal places.

#### 3. Finding max value of console. 2 methods found. 

- Math.max is better for shorter arrays?  Simple example: 
<code> const testArray = [["x", 2], ["y", 7], ["b", 1], ["c", 3], ["a", 5]]; 

let numberArray = []; 
for (i=0; i < testArray.length; i++) {
    numberArray.push(testArray[i][1]); 
}
let max = Math.max.apply(null, numberArray);
console.log(max); </code>

- Use a comparitive function in `.reduce()`

## License

MIT License