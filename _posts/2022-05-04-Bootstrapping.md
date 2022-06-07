---
Layout:
Title:  "Bootstrapping"
Date:   "2022-05-04"
Categories:
---
# introduction
In the HTML5 and CSS section of freeCodeCamp we built a Cat Photo App. Now let's go back to it. This time, we'll style it using the popular Bootstrap responsive CSS framework.
Bootstrap will figure out how wide your screen is and respond by resizing your HTML elements - hence the name responsive design.


# body
With responsive design, there is no need to design a mobile version of your website. It will look good on devices with screens of any width.

You can add Bootstrap to any app by adding the following code to the top of your HTML:

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous"/>
In this case, we've already added it for you to this page behind the scenes. Note that using either > or /> to close the link tag is acceptable.
First, add a new image below the existing one. Set its src attribute to https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg.

It would be great if this image could be exactly the width of our phone's screen.

Fortunately, with Bootstrap, all we need to do is add the img-responsive class to your image. Do this, and the image should perfectly fit the width of your page.
Now that we're using Bootstrap, we can center our heading element to make it look better. All we need to do is add the class text-center to our h2 element.



# conclusion
Remember that you can add several classes to the same element by separating each of them with a space, like this:

<h2 class="red-text text-center">your text</h2>
Bootstrap has its own styles for button elements, which look much better than the plain HTML ones.
