[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11756285&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
console.log(mystery([34,76,45,12,45,65]))
this give us the value of 76. Which is the greatest value.
The mystery function take in an array of integers and checks if the length of the array is equal to 1. 
If so the function returns the value at index 0.
if the length of the arrray is greater than one, the the variable foo which calls the mystery funtion recursively taking in a portion of the array 
from a[1] to the end of the array using the slice function, and checks if the value at the index is greater than the value at a[0].This in tern 
give us the highest value in the array after going through each itteration of the recursive function. 
