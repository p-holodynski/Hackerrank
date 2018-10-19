# Day 7 : Arrays
```javascript
function main() {
    const n = parseInt(readLine(), 10);

    const arr = readLine().split(' ').map(arrTemp => parseInt(arrTemp, 10));
    var reversedArr = arr.reverse();
    console.log(reversedArr.join(" "));
}
```
