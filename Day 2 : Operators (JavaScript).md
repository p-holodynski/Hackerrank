# Hackerrank 30 days of code
Given the meal price (base cost of a meal), tip percent (the percentage of the meal price being added as tip), and tax percent (the percentage of the meal price being added as tax) for a meal, find and print the meal's total cost.
```javascript
// Complete the solve function below.
function solve(meal_cost, tip_percent, tax_percent) {
var tip = (meal_cost * (tip_percent / 100)).toFixed(2);
var tax = (meal_cost * (tax_percent / 100)).toFixed(2);
var result = Math.round(meal_cost + parseFloat(tip) + parseFloat(tax));
console.log(result);
}
```
