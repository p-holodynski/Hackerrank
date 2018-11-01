# Day 14 : Scope
```cs
public Difference(int[] elements){
        this.elements = elements;
    }

    public int computeDifference(){
      maximumDifference = 0;
      for(int i = 0; i < elements.Length; i++){
        for(int j = i; j < elements.Length; j++){
           if(Math.Abs(elements[i] - elements[j]) > maximumDifference){
               maximumDifference = Math.Abs(elements[i] - elements[j]);
           }
        }
      }
      return maximumDifference;
     }
```
