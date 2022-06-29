---
Layout:
Title:  "Solving katas"
Date:   "2022-06-28"
Categories:
---
# introduction
This is the first part. You can solve the second part here when you are done with this. Multiply two numbers! Simple!

The arguments are passed as strings.
The numbers may be way very large
Answer should be returned as a string
The returned "number" should not start with zeros e.g. 0123 is invalid
This is a description of one of the toughest katas I had solved. This is a 4kyu kata and I am not yet on this level. 


# body
const multiply=(a, b)=>  return (BigInt(a) * BigInt(b)).toString();
With this being my solution after asking Mr. Google to help me out with how to handle really large numbers, I discovered the BigInt() method.


# conclusion
Just one of many I have successfully tried and completed.