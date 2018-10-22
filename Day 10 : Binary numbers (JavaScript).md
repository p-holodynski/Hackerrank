# Day 10 : Binary numbers
```javascript
function main() {
    const n = parseInt(readLine(), 10);
    var binary = n.toString(2);
    var arr = binary.split("0");
    var count = 0;
    for(var i = 0; i < arr.length; i++){
        if(arr[i].length > count){
            count = arr[i].length;
        }
    }
    console.log(count);
}
```
