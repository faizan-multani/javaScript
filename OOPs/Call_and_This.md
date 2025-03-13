# call() :
- call() is a method that allows you to invoke a function with a specific this context. The this keyword in JavaScript refers to the object that is currently executing the code, and its value is determined by how a function is called.
```
function SetUsername(username){
    //complex DB calls
    this.username = username
    console.log("called");
}

function createUser(username, email, password){
    SetUsername.call(this, username)
   
    this.email = email
    this.password = password
}

const chai = new createUser("chai", "chai@fb.com", "123")
console.log(chai);
```