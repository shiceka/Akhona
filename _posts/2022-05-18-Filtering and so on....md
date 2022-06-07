---
Layout:
Title:  "Filtering and so on..."
Date:   "2022-05-18"
Categories:
---
# introduction
Another useful array function is Array.prototype.filter(), or simply filter().

filter calls a function on each element of an array and returns a new array containing only the elements for which that function returns true. In other words, it filters the array, based on the function passed to it. Like map, it does this without needing to modify the original array.



# body
The callback function accepts three arguments. The first argument is the current element being processed. The second is the index of that element and the third is the array upon which the filter method was called.

See below for an example using the filter method on the users array to return a new array containing only the users under the age of 30. For simplicity, the example only uses the first argument of the callback.

const users = [
  { name: 'John', age: 34 },
  { name: 'Amy', age: 20 },
  { name: 'camperCat', age: 10 }
];

const usersUnder30 = users.filter(user => user.age < 30);
console.log(usersUnder30); 
The console would display the value [ { name: 'Amy', age: 20 }, { name: 'camperCat', age: 10 } ].
You might learn a lot about the filter method if you implement your own version of it. It is recommended you use a for loop or Array.prototype.forEach().
Concatenation means to join items end to end. JavaScript offers the concat method for both strings and arrays that work in the same way. For arrays, the method is called on one, then another array is provided as the argument to concat, which is added to the end of the first array. It returns a new array and does not mutate either of the original arrays. Here's an example:

[1, 2, 3].concat([4, 5, 6]);
The returned array would be [1, 2, 3, 4, 5, 6].
Functional programming is all about creating and using non-mutating functions.



# conclusion
The last above introduced the concat method as a way to combine arrays into a new one without mutating the original arrays. Compare concat to the push method. push adds an item to the end of the same array it is called on, which mutates that array. Here's an example:

const arr = [1, 2, 3];
arr.push([4, 5, 6]);
arr would have a modified value of [1, 2, 3, [4, 5, 6]], which is not the functional programming way.