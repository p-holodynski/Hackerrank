# Day 6 : Let's review
```javascript
function processData(input) {
    //Enter your code here
    var evenLetters = "";
    var oddLetters = "";
    input = input.split("\n");
    
    for (var i = 1; i < input.length; i++){
    for (var j = 0; j < input[i].length; j++){
        if (j % 2 == 0){
            evenLetters += input[i].charAt(j);
            }
        else{
            oddLetters += input[i].charAt(j);
            }
    }
    console.log(evenLetters + " " + oddLetters);
    evenLetters = "";
    oddLetters = "";
    }
 }
```
