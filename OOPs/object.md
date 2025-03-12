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