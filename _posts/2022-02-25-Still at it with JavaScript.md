---
Layout:
Title:  "Still at it with JavaScript"
Date:   "2022-02-25"
Categories:
---
# introduction
Friday  has been another learning experience as I have continued working on JavaScript, but today it has been arrays which have caught my attention the most. Functions are a great deal important as well, but i shall talk about them on Monday as I am still moving through them.


# body
Arrays are variables which hold more than one element within them. Arrays are declared using square brackets([]), and we get nested arrays which are arrays within arrays and are also known as multidimensional arrays, const arr = [1,2,2,3]; is an array declared with the values 1, 2, 2 and 3. Multidimensional array would be declared as follows: const myArr = [[1,2,3],[4,5,6],7,8,9]. Each element in an array has an index of n-1 meaning that it is a zero based index starting with the first elements index as 0. So if we wanted to call on the first and third element in an array we would use this:
const arr = [50,60,40,55];
arr[0];
const data = arr[2]; the resulting elements called would give us 50 and 40. although the same with multidimensional arrays it does however differ a bit.
const myArr = [[1,2,3],[4,5,6],[7,8,9],10,11,12];
myArr[2];
myArr[2][0];
this would give us the following: [7,8,9]
then for the second one we get 7.
We can add data to the end of an array using .push(x), we can alternatively remove data at the end of an array using .pop().
With that we can add and remove data at the front of an array as well using shift() and unshift() respectively.  



# conclusion
With this new knowledge gained I hope to further extend myself as I start on the functions and proceed on with learning. I had set the goal of starting JS this week and I have done so. Now to go through it and aquire more from it and use it we with the next set of projects. 