---
Layout:
Title:  "Basic data structures"
Date:   "2022-03-18"
Categories:
---
# introduction
We have seen that data can be saved and accessed in different ways. As we already know some of these we can say that arrays and objects are some important ones thus far as they have appeared mosst.

# body
We have seen .push() and .unshift() as methods used to insert data at the end and start of an array respectively. Whilst .pop() and .shift() are methods used to remove data in an array at the end and the beginning respectively. We now see more methods to access data and manipulate it. There is .splice() which we use to remove data entries from arrays, this mmethod can take up to three parameters although mostly we focus on two. They are integers which represent the index, and number of entries to remove from the array the .splice() method is called upon. The third parameter is then an indication of data entries you may want to switch into the position of the entries you have removed.
const numbers = [10,11,12,12,15];
const startIndex = 3;
const numToDel = 1;
numbers.splice(startIndex, numToDel, 13,14);
console.log(numbers);
We will now see that the array numbers = [10,11,12,13,14,15];

Rather than than modifying an array .slice() is a method that allows you to copy a set amount of entries of an array to a new array leaving the array it was called upon untouched.The .slice() method only takes at most two parameters, the first is the index at which we start the extraction and the second is where we stop(this will happen up to but will not include the element at the stop index).
let weather = ['rain','snow','sleet','hail','clear'];
let todaysWeather = weather.slice(1,3);
console.log(todaysWeather);
console.log(weather);
We will get two results on the console the first ['snow','sleet'] and the second ['rain','snow','sleet','hail','clear']. This is to show that the .slice() method made a shallow copy of the original and extracted from that copy without changing the original array. 


# conclusion
We close with the third method which is short but vital too. The method .indexOf() which allows us to quickly and easily check if an element is present in an array. .indexOf() takes an element as a parameterand when called it returns the position or index of that element if present and if not then it returns -1.
function quickCheck (arr, elem){
    if(arr.indexOf(elem)){
        return true;
    }
    return false;
}
This function takes an array and an element as its parameters, it then uses an if statement with the condition that wants the index of the element. It will return true if the element is found and false if not.