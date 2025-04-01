# Object :
-  object is a data structure used to store collections of data and more complex entities. An object is a standalone entity, with properties and types. It's similar to real-life objects, like a car, which might have properties like color, model, and year.
- Properties: Each object has a set of key-value pairs, where the key is a string (often referred to as a property name) and the value can be any valid JavaScript data type (string, number, array, function, other object, etc.).
- Methods: Objects can also contain functions, which are known as methods when they are stored as object properties.

### Example 1 :
```
// singleton
// Object.create

// object literals

const mySym = Symbol("key1")


const JsUser = {
    name: "Hitesh",
    "full name": "Hitesh Choudhary",
    [mySym]: "mykey1",
    age: 18,
    location: "Jaipur",
    email: "hitesh@google.com",
    isLoggedIn: false,
    lastLoginDays: ["Monday", "Saturday"]
}

// console.log(JsUser.email)
// console.log(JsUser["email"])
// console.log(JsUser["full name"])
// console.log(JsUser[mySym])

JsUser.email = "hitesh@chatgpt.com"
// Object.freeze(JsUser)
JsUser.email = "hitesh@microsoft.com"
// console.log(JsUser);

JsUser.greeting = function(){
    console.log("Hello JS user");
}
JsUser.greetingTwo = function(){
    console.log(`Hello JS user, ${this.name}`);
}

console.log(JsUser.greeting());
console.log(JsUser.greetingTwo());
```

### delete a property :
```
let person = {
    name: "John",
    age: 30,
    gender: "male"
};

delete person.gender;  // Deletes the "gender" property
console.log(person);  // { name: "John", age: 30 }
```

## Example 2 :
```
// const tinderUser = new Object()
const tinderUser = {}

tinderUser.id = "123abc"
tinderUser.name = "Sammy"
tinderUser.isLoggedIn = false

// console.log(tinderUser);

const regularUser = {
    email: "some@gmail.com",
    fullname: {
        userfullname: {
            firstname: "hitesh",
            lastname: "choudhary"
        }
    }
}

// console.log(regularUser.fullname.userfullname.firstname);

const obj1 = {1: "a", 2: "b"}
const obj2 = {3: "a", 4: "b"}
const obj4 = {5: "a", 6: "b"}

// const obj3 = { obj1, obj2 }
// const obj3 = Object.assign({}, obj1, obj2, obj4)

const obj3 = {...obj1, ...obj2}
// console.log(obj3);


const users = [
    {
        id: 1,
        email: "h@gmail.com"
    },
    {
        id: 1,
        email: "h@gmail.com"
    },
    {
        id: 1,
        email: "h@gmail.com"
    },
]

users[1].email
// console.log(tinderUser);

// console.log(Object.keys(tinderUser));
// console.log(Object.values(tinderUser));
// console.log(Object.entries(tinderUser));

// console.log(tinderUser.hasOwnProperty('isLoggedIn'));


const course = {
    coursename: "js in hindi",
    price: "999",
    courseInstructor: "hitesh"
}

// course.courseInstructor

const {courseInstructor: instructor} = course

// console.log(courseInstructor);
console.log(instructor);

// {
//     "name": "hitesh",
//     "coursename": "js in hindi",
//     "price": "free"
// }

[
    {},
    {},
    {}
]
```

### Example 3(Methods in object) :
```
let person = {
    name: "John",
    age: 30,
    greet: function() {
        console.log("Hello, my name is " + this.name);
    }
};

person.greet(); // "Hello, my name is John"
```
## Note :
- The ' this ' keyword refers to the object itself (in this case, person).

# more about object :
- Object.keys(), Object.values(), and Object.entries()
- These are useful methods for working with objects.

### Object.keys() :
- Returns an array of the object's property names (keys).
```
let person = {
    name: "John",
    age: 30
};

console.log(Object.keys(person)); // ["name", "age"]
```

### Object.values() :
- Returns an array of the object's property values.
```
let person = {
    name: "John",
    age: 30
};

console.log(Object.values(person)); // ["John", 30]
```

### Object.entries() :
- Returns an array of key-value pairs as arrays.
```
let person = {
    name: "John",
    age: 30
};

console.log(Object.entries(person)); // [["name", "John"], ["age", 30]]
```

## Note :
- The Object.assign() method is used to copy properties from one or more source objects to a target object. It performs a shallow copy.
```
let person = {
    name: "John",
    age: 30
};

let additionalInfo = {
    gender: "male",
    country: "USA"
};

// Copy properties from `additionalInfo` to `person`
Object.assign(person, additionalInfo);
console.log(person); 
// { name: "John", age: 30, gender: "male", country: "USA" }
``` 

# Conclusion :
- Object creation: Can be done using {} or new Object().
- Accessing values: Use dot notation (object.property) or bracket notation (object["property"]).
- Methods: Objects can have methods, which are functions stored as properties.
- Destructuring: Allows unpacking object properties into variables.
- Utility methods: Object.keys(), Object.values(), and Object.entries() help manipulate object data.