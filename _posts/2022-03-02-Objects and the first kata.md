---
Layout:
Title:  "Objects and the first kata"
Date:   "2022-03-02"
Categories:
---
# introduction
Today went a little different from the other days as we had the seniors give us a kata, which is a 
problem we have to solve individually as the juniors. This was interesting cause soon after we had a 
sit down and they started explaining all the work we had done previously.Then i went on to revise 
the work I had touched on with regards to Objects.


# body
The kata is for us to check how much of the work we understand so we will be given these on a regular basis. 
This also allows us to check up on each other as I have realised that some of the juniors I found here are afraid of 
asking for help. They feel they seem to be a disturbance to those they ask for help especially if it is on the regular.

Objects are the talk of the day and in much they are similar to arrays, the difference is that we do not use indexes, but
rather something called properties to access and modify data. Objects store data in a structured way and may be used to portray
real world objects. For each property we have that property's value. We use two ways to access these properties, dot notation(.) 
and bracket notation([]), similar to an array. Dot notation is used when you know the properties name ypu are trying to access well ahead of time. 

let prop1val;
let prop2val; 
const myObj = { 
    prop1 : "val1",
    prop2 : "val2"
}
 prop1val = myObj.prop1;  the value of prop1val is now the string "val1".
 prop2val = myObj.prop2;  the value of prop2val is now the string "val2".

 Then bracket notation is used if the property of the object has a space in its name, although we can still use bracket notation 
 if the property does not have a space in its name.

 let prop1val;
 let prop2val;
 const myObj = {
     "space name" : "Kirk",
     "more space" : "Spock",
     "noSpace" : "USS Enterprise"
 }
prop1val = myObj["space name"];  the value of prop1val is now the string "Kirk".
prop2val = myObj["more space"];  the value of prop2val is now the string "Spock".

Updating objects using dot or bracket notation is in a similar way as to the way we add new properties. To modify :
myObj.noSpace = "USS Enterprise II" 
or myObj["space name"] = "Captain Kirk".
To add a new property :
myObj.space = "USS Raven" or
myObj[" space "] = "USS Raven".


# conclusion
With so much to share we could go on for hours, like checking if a certain property exists in an object or deleting of a property.
There is a great deal still to learn and for me to grasp as the uses required differ and I real world uses vary too. I am still in my learning
phases and hope to teach or help others with most of the concepts I have learnt to use. 