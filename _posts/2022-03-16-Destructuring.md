---
Layout:
Title:  "Destructuring"
Date:   "2022-03-16"
Categories:
---
# introduction
Destructuring assignment is a special syntax which neatly assigns values taken directly from an object. 


# body
const user = { name: "John Doe", age: 54}
const name = user.name;
This has now assigned the value "John Doe" to the new variable name.
const age = user.age; 
This has now assigned the value 54 to the new variable age.
const {name,age} = user; 
Again the new variables have been assigned the values "John Doe" and 54 respectively.
New variable names can be assigned when values are extracted, this is done by putting the new variable name after a colon when assigning the value.
const highTemperatures = {
    yesterday: 75,
    today: 77,
    tomorrow: 80
};
const {today:highToday, tomorrow:highTomorrow} = highTemperatures;

We can extract values of object properties and assign them to variables with the same name. We can also then assign an object properties values to variables with different names.
const user = {johnDoe:{
    age:54,
    email:'johnDoe@yahoo.com'
}};
const {johnDoe:{age,email}} = user;
This is for the same name assignment.
const {johDoe:{age:userAge, email:userEmail}} = user;
This is for different name assignment.



# conclusion
This is hard to grasp as it is somehow confusing ,but understanding all of this is the reason we are here. I shall come back with the rest of this once i understand good and properly. 
