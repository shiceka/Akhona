---
Layout:
Title:  "ECMAScript-6"
Date:   "2022-03-10"
Categories:
---
# introduction
ECMAScript-6 or ES6 is a standardized version of javascript, yet a significant update to the JavaScript programming language. It is a biggest update to the programming language since ES5 which was introduced in 2009. I shall share the little knowledge I have gained at the beginning of this chapter in the programming world.



# body
To prevent object mutation we use Object.freeze(). This prevents any changes whatsoever that will be attempted. 
let obj = {
    name: "Nkosana",
    age: 29,
    gender: "male"
};
Object.freeze(obj);
This is how it is used and will prevent any changes done anywhere down the code. Then we hit a section called arrow functions which has changed a lot of things in terms of my programming. From the way we started with functions this brings about concise programming principals. From this:
const myFunc = function (){                                 const myFunc = () => {
    const myVar = "value";               to this:             const myVar = "value";               
    return myVar;                                             return myVar;
};                                                           };
To make it even better, when there is no function body and only a return value, the syntax of arrow functions has allowance to omit the keyword 'return' as well as the curly brackets ({}) around the code like this:
const myFunc = () => "value"; 
Just like as in a regular function, we can pass arguments into an arrow function, and if we have only one argument then we can also omit the brackets around it.
const myFunc = item => item * 8;
With the above mentioned we can have more than one argument:
const myFunc = (item, add) => item + add;
myFunc(2, 6);

We then hit other amazing section along the way like the rest parameter, which allows a function to take on an adaptable number of arguments. These arguments are then stored in an array, and can be accessed later on within the function.
const sum = (...arg) => arg.reduce((a,b) => a + b, 0;
console.log(sum(1,2,3,4)); The console log will display the number 10 which is the sum of these four numbers that were taken as arguments.   




# conclusion
With so much more to it ES6 really is different and adds more dynamics to javascript, there are things like the 'Spread operator" and destructuring which I am still to go through. The learning curve just got steeper and one needs to start pushing themselve harder. 