---
Layout:
Title:  "Object oriented programming"
Date:   "2022-03-23"
Categories:
---
# introduction
This is one of the biggest sections in the software development process. With object oriented programming, objects and classes organize code and describe things along with what they are capable of.

# body
With objects having a special type of property called mthods, we get to see that methods are in fact properties that are functions. This  adds different behaviour to an object.
let duck ={
    name: "Aflac",
    numLegs: 2,
    sayName: function(){
        return "The name of this duck is " + duck.name + ".";
    }
};
console.log(duck.sayName);
This will return to us the string "The name of this duck is Aflac."
 We can avoid a lot of issues by using the keyword 'this':
 let duck ={
    name: "Aflac",
    numLegs: 2,
    sayName: function(){
        return "The name of this duck is " + this.name + ".";
    }
};
This is a deep topic and the above is the only way to use it. In the current context 'this' refers to the object that the method is associated with: duck. 
Should the name duck be changed to penguin then we need not look for all insatances of duck to change one by one or at all. This makes our code reuseable and easier to read.
Constructors are functions that create new objects. They define properties and behaviours that will belong to the new object. They are usually thought of as the blueprints to the creation of new objects.
const Bird = () => {
    this.name = "Abednego";
    this.colour = "green";
    this.numLegs = 2;
} 

# conclusion
Now constructors sure do look like objects but do have a few differences:
-Constructors are defined with a capitalized name to distinguish the from other functions that are not constructors.
-Constructors use the keyword 'this' to set properties of objects they will create. Inside constructor 'this' refers to a new object it will create.
-Constructors define properties and behaviours intead of returning a value as other functions might. 