---
Layout:
Title:  "Maths and more...plus codewars"
Date:   "2022-03-14"
Categories:
---
# introduction
After Friday I came back with a little more glimour of hope, there is a great amount of light at the end of this tunnel. Such is the challenge of getting there which one has to struggle through, math functionality and the first of codewars are such challenges.


# body
Math.random() is a built in math function with allows us to generate a random number ranging between zero and one. This fantastic function may at anytime return the number 0, but never shall it return the number 1. Let us say we want a random number with a range 0 to 20 this is possible by using a combination of math functions. So we will introduce the Math.floor function which will round off a number down to its whole number. So first we will generate a random decimal number between 0 and 1 using Math.random(), then we will multiply that number by 20, using the Math.floor function we round it down to a whole number. This will look like this:
Math.floor(Math.random() * 20); 
Now we can similarly generate random numbers between a said range:
Math.floor(Math.random() * (max - min + 1)) + min;

We can also interestingly take a string and convert it into an integer using a parseInt() function, which is also built in to the JavaScript language. So if given a number as a string we can pass it into this function which will return to us an integer:
const num = parseInt('007');
The resultant return will be the number 7. Then there is a parseInt() with a radix of which I am still not sure, but it takes the string to be converterd and a radix of which I am to always assume is two into its parameters unless otherwise said. This notaion will look like this:
parseInt(str,radix(assumed to be 2)).


# conclusion
In conclusion of today I was told to join codewars which is a wow place that tests our programming skills and I learnt later on has levels of rating which one has to work up from 8 to 1 hopefully after becoming a great programmer. Gaining skill points and actual skills is the main purpose of this so I feel I am in a good place for now.

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