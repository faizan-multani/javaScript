# IIFE : Immediately Invoked Function Expression.
-  IIFE is a function that is defined and immediately executed.

## Syntax : 
```
()()
```
### Note :
- first ' () ' is for function to perform specific task.
- second ' () ' is used to call function.

```
(function db(){
    // named IIFE
    console.log(`DB CONNECTED`);
})();

( (name) => {
    console.log(`DB CONNECTED TWO ${name}`);
} )('hitesh')
```