# Day 11 : 2D arrays
```javascript
function main() {
    let arr = Array(6);

    for (let i = 0; i < 6; i++) {
        arr[i] = readLine().split(' ').map(arrTemp => parseInt(arrTemp, 10));
    }
    let sumArr = [];
    let centre;
    
    for (let i = 1; i < arr.length - 1; i++){
        for (let j = 1; j < arr[i].length - 1; j++){
            let checker = 0;
            centre = arr[i][j];
            
            //console.log(arr[i-1][j-1] + ' left up');
            //console.log(arr[i-1][j] + ' up');
            //console.log(arr[i-1][j+1] + ' right up');
            //console.log(centre + ' centre');
            //console.log(arr[i+1][j-1] + ' left down');
            //console.log(arr[i+1][j] + ' down');
            //console.log(arr[i+1][j+1] + ' right down');
          checker += arr[i-1][j-1];
          checker += arr[i-1][j];
          checker += arr[i-1][j+1];
          checker += centre;
          checker += arr[i+1][j-1];
          checker += arr[i+1][j];
          checker += arr[i+1][j+1];
          //console.log(checker);
          sumArr.push(checker);
        }
       }
       sumArr = sumArr.sort(function(a,b){return b - a});
       console.log(sumArr[0]);
 }
 ```
