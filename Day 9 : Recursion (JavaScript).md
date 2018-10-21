# Day 9 : Recursion
```javascript
!! not finished !!
function factorial(n, accumulator) {
    if (n === 0){
     return accumulator;
    }
    else {
        return factorial(n - 1, n * accumulator);
    }
}
```
