# LJ Code 201 - Day 18

#### CSS (bg-image fixed when handling corresponding elements)
1. Wrap image you want to display in div (or other)
2. set visibility of image to hidden
3. set image width to 100%
Now the content will flow around the hidden image
1. Set div wrapper to have a background-image: 'your image';
2. give it a fixed/absolute position (so the page scrolls over it)
3. set position/size/repeat respectively

#### Retriving localStorage (arrays)
- you can check if it is an empty array by using </br>
(JSON.parse(localStorage.<i>array</i>)[0]) </br>
and it will return true if there is something in the array </br>
or false if the array is empty
