# Date :
-  Date object is used to work with dates and times. It allows you to create, manipulate, and format dates and times in a variety of ways.

```
let currentDate = new Date();
console.log(currentDate); // Outputs the current date and time
```

```
let date = new Date();

console.log(date.getFullYear());   // Current year (e.g., 2025)
console.log(date.getMonth());      // Current month (0-indexed: 0 = January, 11 = December)
console.log(date.getDate());       // Current day of the month (1-31)
console.log(date.getHours());      // Current hour (0-23)
console.log(date.getMinutes());    // Current minute (0-59)
console.log(date.getSeconds());    // Current second (0-59)
console.log(date.getMilliseconds()); // Current millisecond (0-999)

```

```
// Dates

let myDate = new Date()
// console.log(myDate.toString());
// console.log(myDate.toDateString());
// console.log(myDate.toLocaleString());
// console.log(typeof myDate);

// let myCreatedDate = new Date(2023, 0, 23)
// let myCreatedDate = new Date(2023, 0, 23, 5, 3)
// let myCreatedDate = new Date("2023-01-14")
let myCreatedDate = new Date("01-14-2023")
// console.log(myCreatedDate.toLocaleString());

let myTimeStamp = Date.now()

// console.log(myTimeStamp);
// console.log(myCreatedDate.getTime());
// console.log(Math.floor(Date.now()/1000));

let newDate = new Date()
console.log(newDate);
console.log(newDate.getMonth() + 1);
console.log(newDate.getDay());

// `${newDate.getDay()} and the time `

newDate.toLocaleString('default', {
    weekday: "long",
    
})
```