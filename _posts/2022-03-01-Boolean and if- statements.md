---
Layout:
Title:  "Boolean and if statements"
Date:   "2022-03-01"
Categories:
---
# introduction
Well today was a good day as I managed to push through most of the work on freecode camp as well as 
manqaging to get through a problem I was stuck on yesterday. With the help of my class mates we were able 
to overcome. The one topic I will touch on is the boolean and the "if statement".


# body
After learning that the boolean is a data type that can only be either true or false. These two may be dipicted 
as on for true and off for false, and these states are said to be mutually exclusive. Then we moved on to 
"if statements" of which i found to also interesting for they are simple at first, but may throw you off at some point.
if( condition is true ) {
    statement is executed
}
With these we have assignment operators, comparison operators and strict comparison operators.
= is the first of such and is the assignment operator,
== this is the comparison operator and converts either value(operand) to its right or left to a common type,
=== this is the strict comparison operator and this does no type conversion of its operands. 
1 == 1 will test true. 
1 == 2 will test false.
1 == "1" will test true even though the quoted 1 is a string thus the type conversion is pereformed.
1 === 1 will test true.
1 === "1" will test false, no type conversion.
Alternatively we can use "typeof" to determine the variable type.
if(num > 5 && num < 10){
    return true;
} else{
return false;
} 
The above statement says that if a number is greater than 5 and also smaller than 10 then it should return 
the boolean true, else if not true then it should return the boolean false. Also we have used the logical 
"and" operator which requires both the operands to its right and left to be true. 


# conclusion
Having learnt this means that comparing statements is simple and having alternatives in a situation can now be easily 
put into code and have our program give the user different answers for different statements.