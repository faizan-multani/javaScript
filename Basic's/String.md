# String : 
- strings are used to represent sequences of characters (text). Strings are one of the primitive data types.

## key Point :
- Immutability : Strings in JavaScript are immutable, meaning once a string is created, it cannot be modified. Any operations on a string return a new string, not modifying the original string.
- Indexed : Each character in a string has an index, starting at 0 for the first character.
- Length: You can easily find the length of a string using the .length property.

## Example with string methods :
```
const name = "hitesh"
const repoCount = 50

// console.log(name + repoCount + " Value");

console.log(`Hello my name is ${name} and my repo count is ${repoCount}`);

const gameName = new String('hitesh-hc-com')

// console.log(gameName[0]);
// console.log(gameName.__proto__);


// console.log(gameName.length);
// console.log(gameName.toUpperCase());
console.log(gameName.charAt(2));
console.log(gameName.indexOf('t'));

const newString = gameName.substring(0, 4)
console.log(newString);

const anotherString = gameName.slice(-8, 4)
console.log(anotherString);

const newStringOne = "   hitesh    "
console.log(newStringOne);
console.log(newStringOne.trim());

const url = "https://hitesh.com/hitesh%20choudhary"

console.log(url.replace('%20', '-'))

console.log(url.includes('sundar'))

console.log(gameName.split('-'));
```