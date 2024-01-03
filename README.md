<h1 align='center'>
Character Concatenation
</h1>
<h3>
Description
</h3>
<text>
Given a string, you progressively need to concatenate the first letter from the left and the first letter to the right and "1", then the second letter from the left and the second letter to the right and "2", and so on.

If the string's length is odd drop the central element.
</text>

<h3>
Solution
</h3>
```
function charConcat(string){
 
  let myString = string.split("");
  
  let myArray = [];
  
  for (let i=1; i<=myString.length/2 ;i++ ){

    myArray.push(myString[i-1])
 
    myArray.push(myString[myString.length-i])

    myArray.push(i)
  }

   return myArray.join("")
}
<h3 align='center'>
[Kata](https://www.codewars.com/kata/55147ff29cd40b43c600058b)
</h3>