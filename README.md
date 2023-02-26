# Financial Analysis
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Link to site

https://daisyeverard.github.io/console-financial-analysis/

## Preview

<p align="center">
  <img src="./assets/preview.png" width="800" alt="screenshot of site">
</p>

## Table of Contents

- [Description](#description)
- [Calculations](#calculations)
- [Technologies](#technologies)
- [Issues and Solutions](#issues-and-solutions)
- [Contacts](#contacts)

## Description
This is a tool to analyse an array of finanacial data with months and years provided in nested arrays. The output is: 
1. The number of months covered
2. The Net profit over that period
3. The average profit per month
4. The average change in profit per month
5. The month with and value of the greatest profit
6. The month with the greatest increase
7. The month with and value of the greatest profit
8. The month with the greatest decrease

## Calculations
1. finances.length
2. `for` loop adding all profits
3. `2/1` To round to 2dp and show a value with a precision up to cents in a dollar, `toFixed(2)` was used
4. From index 1 of `finance`, sum (this month - last month)
5. `numberArray` was created with a for loop to store only numerical values and remove months
`Math.max()` assigned the highest value in `numberArray` to new variable `max`.
Another for loop then found the month that `max` corresponded to and assigned that month (string) to `dateOfMax`;
6. `changeArray` created using (this month - last month) figures. `Math.max()` for greatest value. This time the for loop finds one index higher in `finance` than in `changeArray`, as the first index of `finance` was omitted when creating `changeArray`.
7. Same as 5 but with min, `numberArray` already defined.
8. Same as 6 but with min, `changeArray` already defined.

## Technologies

- HTML
- JavaScript

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

## Contacts

- GitHub: [DaisyEverard](https://github.com/DaisyEverard)
- LinkedIn: [daisy-everard](https://www.linkedin.com/in/daisy-everard/)
- Email: msdeverard@gmail.com


## License

MIT License
