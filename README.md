This project is part of the web performance part of Udacity's Front-End Web Development Nanodegree.

Specifically I did the following changes:

Speed of loading part:
- Inlined CSS.
- Added the print media query to the print.css file.
- Added async tag to the google analytics js file.
- Compressed and resized images.



Pizza 60 frames part:
- Avoided repeated code. For example, queries like "document.querySelectorAll(".randomPizzaContainer")" are unnecessarily repeated.
- Reduced the number of pizza images moving in the animation. In the original project there were 200 and most of them were animating off screen.
- Switched from the left propert to a "transform: translateX" in the pizza animations.
- Some fixed values were being unnecessarily read within loops. For example, the updatePositions() function had "document.body.scrollTop" happening in every iteration of the loop.
