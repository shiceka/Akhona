---
Layout:
Title:  "Regular Expressions"
Date:   "2022-03-15"
Categories:
---
# introduction
Regular expressions or regex are used in programming languages to match parts of strings. One has to create patterns to help them do the matching. If we wanted to find the word "the" in the string, 'The dog chased the cat', we would use the following regex: /the/;.One can notice that quotation marks are not required in regex.


# body
Now there are some methods in regex which help us out, one of these is the .test() method. This method takes the regex and applies or tests it against the string and returns true or false if the pattern is found or not respectively.
let testStr = 'freeCodeCamp';
let testRegex = /Code/;
let result = testRegex.test(testStr);
console.log(result); //The test method will return the value true.
To match a variety of possibilites we use the alternation or OR operator: | for example /yes|no|maybe/ this is to look for either before or even after the operator.
Regex is case sensitive, but as with most programming there are ways around that. We can get by this using flags, like the case sensitive flag 'i' which ignores case. We use this flag by appending it to the regex : /ignorecase/i; This regex will match the strings ignorecase, igNoreCase and IgnoreCase.
There is a method that we use to extract actual matches found .match() method. To use this method we apply it on a string and pass the regex inside its parenthesis like this:
let ourStr = 'Regular expressions';
let ourRegex = /expressions/;
let result = ourStr.match(ourRegex);
console.log(result); // This will return ["expressions"].
Note that .test() and .match() syntax are opposites of each other:
'string'.match(/regex/);
/regex/.test('string');

# conclusion
There is another flag in regex that is called the global flag 'g' which allows us to extract or search for more than one instance of the pattern. And we also have a wild card which we use in case do not know all the characters in a pattern. This wildcard is known as the dot or period and is used like this:
let humStr = 'I'll hum a song';
let hugStr = 'Bear hug';
let hutStr = 'I have a beautiful Hut';
let huRegex = /hu./gi; //used with the two flags 
huRegex.test(humStr);
huRegex.test(hugStr);
huRegex.test(hutStr);
All three results will return as true thanks to the wildcard and the flags.