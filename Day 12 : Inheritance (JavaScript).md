# Day 12 : Inheritance
```javascript
class Student extends Person {
    /*	
    *   Class Constructor
    *   
    *   @param firstName - A string denoting the Person's first name.
    *   @param lastName - A string denoting the Person's last name.
    *   @param id - An integer denoting the Person's ID number.
    *   @param scores - An array of integers denoting the Person's test scores.
    */
    // Write your constructor here
    constructor(firstName, lastName, id, scores) {
        super();
        this.firstName = firstName;
        this.lastName = lastName;
        this.idNumber = id;
        this.scores = scores;
    }
    /*	
    *   Method Name: calculate
    *   @return A character denoting the grade.
    */
    // Write your method here
    calculate(){
       let sum = 0;
       for (let i = 0; i < this.scores.length; i++){
            sum += this.scores[i];
       }
       let avg = sum / this.scores.length;
       //console.log(avg);
       if(90 <= avg && avg <= 100){
            return "O";
       }
       if(80 <= avg && avg < 90){
            return "E";
       }
       if(70 <= avg && avg < 80){
            return "A";
       }
       if(55 <= avg && avg < 70){
            return "P";
       }
       if(40 <= avg && avg < 55){
            return "D";
       }
       if(40 > avg){
            return "T";
       }
    }
}
```
