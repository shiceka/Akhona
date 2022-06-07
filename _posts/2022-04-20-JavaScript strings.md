---
Layout:
Title: "JavaScript strings"
Date: "2022-04-20"
Categories:
---

# introduction

A string literal, or string, is a series of zero or more characters enclosed in single or double quotes.
After declaring a variable we can assign it a string like this : var myStr = "Hey my name is Bob the cat";

# body

In JavaScript, you can escape a quote from considering it as an end of string quote by placing a backslash (\) in front of the quote. This is simply because quotes and strings use the same double or single quotes. So for example if we hava a string : var sampleStr = "Noxolo said, \"Kamva and Lindo are good at explaining JavaScript\".";
This will signal to JavaScript that the quote is not the end of the string, but instead may have to appear inside the string. So if you were to print this we would get: Noxolo said, "Kamva and Lindo are good at explaining JavaScript".
Quotes are not the only characters that can be escaped inside a string. There are two reasons to use escaping characters:
1. To allow you to use characters you may not otherwise be able to type out, such as a carriage return.
2. To allow you to represent multiple quotes in a string without JavaScript misinterpreting what you mean.

  Code	 Output
1. \'	  single quote
2. \"	  double quote
3. \\	  backslash
4. \n	  newline
5. \r	  carriage return
6. \t	  tab
7. \b	  word boundary
8. \f	  form feed

We can find the length of a String value by writing .length after the string variable or string literal. Bracket notation is a way to get a character at a specific index within a string. Most modern programming languages, like JavaScript, don't start counting at 1 like humans do. They start at 0. This is referred to as Zero-based indexing. For instance, the character at index 0 in the word Njabulo is the N. 
var firstName = "Muano", you can get the value of the first letter of the string by using firstName[0]. 
You can also use bracket notation to get the character at other positions within a string. In order to get the last letter of a string, you can subtract one from the string's length: firstName[firstName.length - 1]. You can use the same principle we just used to retrieve the last character in a string to retrieve the Nth-to-last character: firstName[firstName.length - 3] this will get us the third to last character. 

# conclusion
Now it is also good to note that a single character in a string can not be change unless we change the whole string:
let myName = "Mondli"; can not be changed as follows... 
myName[0] = "W'; but as staed above may be changed to a completely new string. 
myName = "Wondli"; this is acceptable as strings are said to be immutable.
