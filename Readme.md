# Task 10: CSS Animation to Hero Image

**Author:** D P Rithvik Kumar

## Description & Learning Process
This assignment challenged me to create a continuous orbital animation with a squeezing effect for the main hero image. 

I honestly struggled with the geometry of CSS transforms on this one. My first attempt was just using standard `translate()` values to move the image up, down, left, and right. But when I tested it in the browser, the image was moving in a rigid square/diamond path, not a smooth circle. 

After some serious testing and debugging, I learned a really cool CSS trick for true circular orbits: you have to combine `rotate` and `translate` simultaneously. By rotating the element forward (e.g., `rotate(90deg)`), pushing it out from the center with `translateX(30px)`, and then immediately rotating it *backward* by the same amount (`rotate(-90deg)`), the image moves in a perfect circle while staying upright! I combined this math with the `scale()` property at the 25% and 75% keyframes to give it the squishy, squeezed effect required by the prompt.

## How to Run (Local Testing)
1. Download or clone this project folder to your local machine.
2. Verify that `index.html`, `style.css`, and `script.js` (blank) are all properly linked and located in the same root directory.
3. Double-click `index.html` to open it in your default web browser.
4. Watch the main washing machine hero image. You will see it moving in a true circular orbit while smoothly squeezing and stretching as it moves along the path.
