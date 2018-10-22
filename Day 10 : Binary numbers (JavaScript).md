# Day 10 : Binary numbers
```javascript
function main() {
    const n = parseInt(readLine(), 10);
    var binary = n.toString(2);
    var count = 1;
    for(var i = 1; i < binary.length; i++){
        if(binary.charAt(i) === binary.charAt(i - 1)){
            count++;
        }
    }
    console.log(count);
}
```
