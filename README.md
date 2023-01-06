# Financial Analysis

## Link to site

https://daisyeverard.github.io/console-financial-analysis/

## Description / How it works
This is a tool to analyse an array of finanacial data with months and years provided in nested arrays. The output is: 
1. The number of months covered
2. The total profit over that period
3. The average profit per month
4. The month with and value of the greatest profit
5. The month with and value of the greatest profit

Calculation of the values: 
1. finances.length
2. `for` loop adding all profits
3. `2/1` To round to 2dp and show a value with a precision up to cents in a dollar, `toFixed(2)` was used
4. `numberArray` was created with a for loop to store only numerical values and remove months
`Math.max()` assigned the lowest value in `numberArray` to new variable `max`.
Another for loop then found the month that `max` corresponded to and assigned that month (string) to `dateOfMax`; 
5. Same as `4` except `numberArray` doesn't need defining again, and changing all mentions of `max` to `min`. 

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
