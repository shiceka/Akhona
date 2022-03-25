---
Layout:
Title:  "ES6 revisited"
Date:   "2022-03-22"
Categories:
---
# introduction
We touched on this before but something caught me and I would like to go through it again as I have come to have a better understanding upon comparison of its use. The spread operator.

# body
Spread operator allows us to expand arrays and other expressions in places where multiple parameters or elements would be expected. 
const arr1 = ['Jan','Feb','Mar',"Apr','May'];
let arr2 = [];
for us to copy all the contents of arr1 into arr2 using the spread operator is:
arr2 = [...arr1];
conole.log(arr2);
We will see ['Jan','Feb','Mar',"Apr','May'].
Now one key difference between the spread operator and array destructuring is that the spread operator unpacks all contents of an array into a comma-seperated list. Consequently , we can not pick and chose which elements we want to assign to variables. Destructuring an array though lets us do exactly that:
const [a,b] = [1,2,3,4,5,6,];
console.log(a,b); 
We will see on display that the values of 'a' and 'b' are '1' and '2', in this example 'a' is assigned the first value and 'b' the second, but we can select a different index in the array with destructuring using commas:
const [a,b,,,c] = [1,2,3,4,5,6];
console.log(a,b,c); 
We will see that on the console the values for 'a','b' and 'c' to be the numbers '1','2' and '5'.  

# conclusion
In closing I would like to say that we can also exchange values of variables:
let a = 8;
let b = 6;
[b,a] = [a,b];
console.log(a,b);
We see that 'a' now holds the value '6' and 'b' holds '8'.