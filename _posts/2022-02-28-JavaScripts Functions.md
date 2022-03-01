---
Layout:
Title:  "JavaScripts Functions"
Date:   "2022-02-28"
Categories:
---
# introduction
Today was not as productive as I would have loved. Working on FreeCode camp for most of the day hasn"t really worked out good. 
I worked on Functions today and that is what I will be sharing on.


# body
function functionName() { console.log("Hello World");} this is the declaration of a function which when called will print
 'Hello World' on the console. Functions may have parameters which are placeholders for values to be input to a function when
 called. These parameters which are passed into a function are called arguments.
 function functionName(param1, param2) {
     console.log(param1 + param2);
 }
When we call this function we should do so having placed two arguments. functionName(7,10); On the console we will see the number 17.
We then have a return statement which is put into a function and will do as its name says return a value back out of the function.
function functionName(val){ return val + 5;} we should get the argument we will insert added to the number 5 returned to us. so if I
call the function : functionName(4); we will have the number 9 returned to us.


# conclusion
As I conclude on this I am yet to properly understand global and local declarations and functions as this notion still slightly eldues me sometimes.
 I do however know that it is better to have both global and local scope in a function, although with this the local variable will take presedence