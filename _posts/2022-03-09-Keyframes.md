---
Layout:
Title:  "@Keyframes"
Date:   "2022-03-09"
Categories:
---
# introduction
I had always wondered growing up and even now as a young adult as to how animation is created. Thought it 
was always drawn then it would have to go to some company so it could be put into a machine to work and come to life.
I then grew and understood that one could create an animation by themselves using programming. I thought I would ask a 
professional, but it seems I do not have to go to those lengths.


# body
I got to TCG and going through the bootcamp there was a section to animate objects, this was through keyframes. So I went 
back recently and looked through the section again. I have to say that I feel like I have achieved something from whence I
was a child. Keyframes rule are specifications of code for animation, created by slowly changing from a set of style in CSS to another.
An animation can be changed a great amount of times ranging from 0% all the way through to 100%. This has to be done whilst having given
the animation a duration, animation iteration count and animation timing function. The duration is a specification as to how long the ani-
mation will run. The iteration count sets the number of times the animation will be played before it stops, it can be set from once all the way to infinity. The timing function is used to control the animation speed and has four settings with the fifth a none specific setting. These are the default setting known as 
ease - which lets the animation start slow, build up speed and then slow down just before the end. 
ease-out - which starts out fast and then slows down at the end.
ease-in - which starts slow and speeds up through to the end.
linear - which has a constant motion from the beginning to the end of the animation. These would be the speeds of an animated car for example in the animation.
cubic-bezier - this has the chance to be any one of the above mentioned as it uses coordinates to determine the motion of the animation.   
Keyframes have a general syntax to work through and looks like :

@keyframes (animation-name) {
    0% {
        styles
    }
    50% {
        styles
    }
    100% {
        styles
    }
}
Animation-name is the name that one can give to their animation and can be any name they choose.
Styles are the cascading style sheets' styling propeties. These set the background of the opening scene all the way to what it looks like half way and then what 
it looks like just before the credits at the end.

# conclusion
With this I have come to the end of the Keyframes talk. Discussed are just several main topics of keyframes and animation properties to explain the way in which simple keyframe animations work. By utilizing some different keyframes and css animation properties, we can better understand the concepts. I hope to play around and get a better feel for animating on my web pages in future.
