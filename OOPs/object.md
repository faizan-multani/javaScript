# Object :
- collection of properties and methods.
- object is a collection of key-value pairs.
- Properties can hold any value (primitive types, arrays, functions, other objects).
- eg. toLowerCase.

# Object Literal : 
- Constructor function
- Prototypes
- Classes
- Instances (new, this)

# syntax :
- using literals
```const person = { // literal
  name: "John", 
  age: 30,   
  greet: function() {
    console.log("Hello, " + this.name);
  }
};
```
- usnig new object()
```
const person = new Object();
person.name = "John";
person.age = 30;
person.greet = function() {
  console.log("Hello, " + this.name);
};
```

## how to access object properties :
- Dot notation
- Bracket notation(square braces)

## Add and Modify values :
```
person.city = "New York"; // Add a new property
person["age"] = 31; // Modify an existing property
```

## Delete property :
- using 'delete' keyword
```
delete person.age; // Removes the 'age' property
```

## Nested object :
```
const car = {
  make: "Toyota",
  model: "Corolla",
  engine: {
        type: "V6",
        horsepower: 200
        }
};

console.log(car.engine.type); // Output: V6
```

```
function multipleBy5(num){

    return num*5
}

multipleBy5.power = 2

console.log(multipleBy5(5));
console.log(multipleBy5.power);
console.log(multipleBy5.prototype);

function createUser(username, score){
    this.username = username
    this.score = score
}

createUser.prototype.increment = function(){
    this.score++
}
createUser.prototype.printMe = function(){
    console.log(`price is ${this.score}`);
}

const chai = new createUser("chai", 25)
const tea = createUser("tea", 250)

chai.printMe()
```
- Here's what happens behind the scenes when the new keyword is used:

A new object is created: The new keyword initiates the creation of a new JavaScript object.

A prototype is linked: The newly created object gets linked to the prototype property of the constructor function. This means that it has access to properties and methods defined on the constructor's prototype.

The constructor is called: The constructor function is called with the specified arguments and this is bound to the newly created object. If no explicit return value is specified from the constructor, JavaScript assumes this, the newly created object, to be the intended return value.

The new object is returned: After the constructor function has been called, if it doesn't return a non-primitive value (object, array, function, etc.), the newly created object is returned.