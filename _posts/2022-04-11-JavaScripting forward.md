---
Layout:
Title:  "JavaScripting forward"
Date:   "2022-04-11"
Categories:
---
# introduction
I started out with finishing off the rest of the JavaScript challenges on the intermediate algorithms section. I had missed most of the previous week due to flu and fear of it being possibly covid.

# body
I came back and finished three of the five problems with the Ceasars cipher being the most fun of them thus far I have even written down the solution cause wow. 
const Rot13=str=>{
    let alphabet = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
    let currentValue ='';
    for(let i = 0; i < str.length; i++){
        if(alphabet.indexOf(str[i]) >= 13){
            currentValue += alphabet[alphabet.indexOf(str[i]) -13]
        }
        else if(alphabet.indexOf(str[i] < 13 && alphabet.indexOf(str[i]) > -1)){
            currentValue += alphabet[aplhabet.indexOf(str[i]) + 13]
        }
        else{
            currentValue += str[i];
        }
    }
    return currentValue;
}
this is the one problem I enjoyed getting through, esplecially after feeling refreshed and not bed ridden or sick. It felt like a breath of fresh air.


# conclusion
Today was a new view at the problems and work done here so I am taking things on differently and facing the days challenges on a positive light regardless. Tomorrow I start with Front end development.