# Day 8 : Dictionaries and Maps
```javascript
function processData(input) {
    //Enter your code here
    input = input.split("\n");
    var entries = parseInt(input[0]);
    var book = input.slice(1, entries + 1);
    var dict = {};
    for (var i = 0; i < book.length; i++){
        var temp = book[i].split(" ");
        dict[temp[0]] = temp[1];
    }
    for (var j = entries + 1; j < input.length; j++){
        if (dict.hasOwnProperty(input[j])){
        console.log(input[j] + "=" + dict[input[j]]);
        }
        else{
         console.log("Not found");
        }
    }
}
```
