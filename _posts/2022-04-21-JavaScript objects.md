---
Layout:
Title:  "JavaScript objects"
Date:   "2022-04-21"
Categories:
---
# introduction
Objects are similar to arrays, except that instead of using indexes to access and modify their data, you access the data in objects through what are called properties. Objects are useful for storing data in a structured way, and can represent real world objects, like a house.
const house = {
  "type": "double-story",
  "doors": 8,
  "number of windows": 29,
  "floors": ["ground", "upper"]
};


# body
However, you can also use numbers as properties. You can even omit the quotes for single-word string properties, if your object has any non-string properties, JavaScript will automatically typecast them as strings. There are two ways to access the properties of an object: dot notation (.) and bracket notation ([]), similar to an array. Dot notation is what you use when you know the name of the property you're trying to access ahead of time.
let myObj = house.type; 
myObj would now have the value of "double-story". 
The second way to access the properties of an object is bracket notation ([]). If the property of the object you are trying to access has a space in its name, you will need to use bracket notation. However, you can still use bracket notation on object properties without spaces.
house["doors"]; this would be the integer 8.
house["number of windows"]; this would be the integer 29. 
Note that property names with spaces in them must be in quotes (single or double). 
After you've created a JavaScript object, you can update its properties at any time just like you would update any other variable. You can use either dot or bracket notation to update.
const ourDog = {
  "name": "Kayla",
  "legs": 4,
  "tails": 1,
  "friends": ["Sesh", "Rex"]
};
Here's how we update this object's name property: ourDog.name = "Spotless Spot"; or ourDog["name"] = "Spotless Spot"; Upon our evaluation of the new or rather old name ourDog.name, instead of getting Kayla, we'll get his new name, Spotless Spot. 


# conclusion
We can also delete properties from objects like this:
const ourDog = {
  "name": "Kayla",
  "legs": 4,
  "tails": 1,
  "friends": ["Sesh", "Rex"]
};
delete ourDog.friends; After that ourDog object will look like this once we console it.  
const ourDog = {
  "name": "Kayla",
  "legs": 4,
  "tails": 1  
};
