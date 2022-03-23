---
Layout:
Title:  "Regular expressions continued"
Date:   "2022-03-17"
Categories:
---
# introduction
The last time we were on this topic we ended with the wildcard and two flags. Now we continue from there and hope to touch on other uses as this is useful for exception handling I would like to think.


# body
We can search for literal patterns with some flexibility and character classes. These allow us to define a group of characters we wish to match by placing them inside square brackets ([]). If we want to match bag,bug,big but not bog, we create the regex/b[aui]g/ for this search. [aui] is the character class that will match only a,u and i.
let bigStr = 'big';
let bugStr = 'bug';
let bagStr = 'bag';
let bogStr = 'bog';
let bgRegex = /b[iua]g/;
bigStr.match(bgRegex);
bugStr.match(bgRegex);
bagStr.match(bgRegex);
bogStr.match(bgRegex);
In the order we have tried to match them we will get the returned results being:
['big'],['bug'],['bag'] and null. Inside a character set we can define a range of characters to match using a hyphen. We can match lowercase letters a through to e like: [a-e]. Using the hyphen we can both numbers and letters like [a-z0-9] with the addition of our flags at the end. We can create a negated character set as well using the caret character(^) just after the opening barcket and before the characters we do not want.:
/[^aeiou]/gi;
This will match all none vowel characters, also worthy to know that '.,!,[,@,/ and white space will be matched.



# conclusion
There are short hand notations for some of these regular expressions which one should look into as they are interesting especially in combinations. This section was a challenge although interesting in its own way. 
