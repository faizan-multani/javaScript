# Array sorting (ascendind order):
```
let arr = [300,8,900,6,400]
let AscArr = arr.sort((a,b) => a-b); // Ascending order
let DescArr = arr.sort((a,b) => b-a) //  Descending order
console.log(newArr)
```
## Output :
```
[ 6, 8, 300, 400, 900 ] ascsending
[ 900, 400, 300, 8, 6 ] descending
```

# find the duplicate values from an arrayb and store it in new array?
```
// const num = [10, 22, 10, 36, 79, 17, 28, 19, 36, 17,10];

const str = ["ajay","john",'mathew',"cesor","cena","mathew","ajay"]

const duplicates = str.filter((item, index) => str.indexOf(item) !== index);
const uniqueDuplicates = [...new Set(duplicates)];

console.log(uniqueDuplicates); 
// Output: [10, 36, 17]
// Output: [ 'mathew', 'ajay' ]
```