---
Layout:
Title:  "Filter, map and reduce"
Date:   "2022-04-01"
Categories:
---
# introduction
The .map() method creates a new array by transforming every element in an array individually. The .filter() method creates a new array by removing elements that don't belong in the filter instance. The .reduce() method on the other hand takes all of the elements in an array and reduces them into a single value. Just like map and filter , reduce is defined on Array.


# body
.map():
Let me explain how it works with a simple example. Say you have received an array containing multiple objects – each one representing a person. The thing you really need in the end, though, is an array containing only the id of each person.
const officers = [
  { id: 20, name: 'Captain Piett' },
  { id: 24, name: 'General Veers' },
  { id: 56, name: 'Admiral Ozzel' },
  { id: 88, name: 'Commander Jerjerrod' }
];
const officersIds = officers.map(officer => officer.id);
So how does .map() work? Basically is takes 2 arguments, a callback and an optional context (will be considered as this in the callback). The callback runs for each value in the array and returns each new value in the resulting array. Keep in mind that the resulting array will always be the same length as the original array.
.filter()
What if you have an array, but only want some of the elements in it? That’s where .filter() comes in!
const pilots = [
  {
    id: 2,
    name: "Wedge Antilles",
    faction: "Rebels",
  },
  {
    id: 8,
    name: "Ciena Ree",
    faction: "Empire",
  },
  {
    id: 40,
    name: "Iden Versio",
    faction: "Empire",
  },
  {
    id: 66,
    name: "Thane Kyrell",
    faction: "Rebels",
  }
];
Say we want two arrays one for rebel pilots and the other for imperial pilots:
const rebels = pilots.filter(pilot => pilot.faction === "Rebels");
const empire = pilots.filter(pilot => pilot.faction === "Empire");
Basically, if the callback function returns true, the current element will be in the resulting array. If it returns false, it won’t be.
.reduce()
Just like .map(), .reduce() also runs a callback for each element of an array. The difference is that reduce passes the result of this callback (the accumulator) from one array element to the other.
The accumulator can pretty much be any data type: integer, string or an object and must be passed when calling .reduce():
const pilots = [
  {
    id: 10,
    name: "Poe Dameron",
    years: 14,
  },
  {
    id: 2,
    name: "Temmin 'Snap' Wexley",
    years: 30,
  },
  {
    id: 41,
    name: "Tallissan Lintra",
    years: 16,
  },
  {
    id: 99,
    name: "Ello Asty",
    years: 22,
  }
];
We need to know the total years of experience of all of them. Notice at that we have set the starting value as 0. Afte`r running the callback for each element of the array, reduce will return the final value of our accumulator (in our case: 82):
const totalYears = pilots.reduce((acc, pilot) => acc + pilot.years, 0);


# conclusion
Combining .map(), .reduce(), and .filter()
Since all three are called on arrays and since .map() and .filter() both return arrays, we can easily chain our calls.
const personnel = [
  {
    id: 5,
    name: "Luke Skywalker",
    pilotingScore: 98,
    shootingScore: 56,
    isForceUser: true,
  },
  {
    id: 82,
    name: "Sabine Wren",
    pilotingScore: 73,
    shootingScore: 99,
    isForceUser: false,
  },
  {
    id: 22,
    name: "Zeb Orellios",
    pilotingScore: 20,
    shootingScore: 59,
    isForceUser: false,
  },
  {
    id: 15,
    name: "Ezra Bridger",
    pilotingScore: 43,
    shootingScore: 67,
    isForceUser: true,
  },
  {
    id: 11,
    name: "Caleb Dume",
    pilotingScore: 71,
    shootingScore: 85,
    isForceUser: true,
  },
];
What we want to get is the total score of personnel able to use force. First, filter out the personnel who can’t use the force. With that we have 3 elements left in our resulting array. We now need to create an array containing the total score of each Jedi. And finally we add the total scores of these jedi.
const totalJediScore = personnel
  .filter(person => person.isForceUser)
  .map(jedi => jedi.pilotingScore + jedi.shootingScore)
  .reduce((acc, score) => acc + score, 0);