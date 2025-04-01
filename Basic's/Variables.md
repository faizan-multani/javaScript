# Variable :
- variable is a container which is used to store the data/value.
- data/value can be changed.

## Rules :
- variable names are case sensitive.
- eg. myVar, MyVar both are different.
- it must begin with letter, _ and $.
- it should not start with number.
- it cannot be a reserved keyword.
- eg. class, let, return, if, try etc.
```
const accountId = 144553
let accountEmail = "hitesh@google.com"
var accountPassword = "12345"
accountCity = "Jaipur"
let accountState;

// accountId = 2 // not allowed


accountEmail = "hc@hc.com"
accountPassword = "21212121"
accountCity = "Bengaluru"

console.log(accountId);

/*
Prefer not to use var
because of issue in block scope and functional scope
*/


console.table([accountId, accountEmail, accountPassword, accountCity, accountState])
```
## in the console , used 'console.table' so data will be in the form of table.

# Difference between var,let and const :

![Image Description](assets/variables.png)

# Variable Hoisting :
- hoisting refers to the behavior where variable declarations (and sometimes function declarations) are moved to the top of their scope during the compile phase, before the code has been executed.

- eg. with var :

```
console.log(x);  // undefined (hoisted but not yet initialized)
var x = 5;
console.log(x);  // 5 (now initialized)
```

- eg. with let/const :
```
console.log(x);  // ReferenceError: Cannot access 'x' before initialization
let x = 5;
console.log(x);  // 5
```

### Note 1 :
- if we define variables hoisting with ' var ' will get undefine as output.
- if define variable hoisting with ' let and const ' will get ' RefferenceError ' because there are in ' temporal dead zone '.

### Note 2 :
- Object property can be changed/updated using ' Const ' variable.
```
const obj = {
    name:'alice'
};

obj.name = 'john'
console.log(obj.name)
```