# Constructor :
- a constructor is a special function used to create and initialize objects. It’s typically used with the new keyword to create instances of an object from a class or function. Constructors allow you to initialize an object's properties and methods when the object is created.
```
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  // Method inside the class
  greet() {
    console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
  }
}

// Creating an instance of Person using the 'new' keyword
const person1 = new Person("John", 25);
const person2 = new Person("Jane", 30);

// Accessing properties and methods
person1.greet(); // Output: Hello, my name is John and I am 25 years old.
person2.greet(); // Output: Hello, my name is Jane and I am 30 years old.
```