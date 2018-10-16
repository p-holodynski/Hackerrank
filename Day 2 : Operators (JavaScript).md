# Hackerrank 30 days of code
``javascript
// Complete the solve function below.
function solve(meal_cost, tip_percent, tax_percent) {
var tip = meal_cost * (tip_percent / 100);
var tax = meal_cost * (tax_percent / 100);
var result = parseInt(meal_cost + tip + tax);
    
    console.log(result);
}
``
