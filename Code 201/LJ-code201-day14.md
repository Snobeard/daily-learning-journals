# LJ Code 201 - Day 14
<a href="../README.md">`Home`</a>
<a href="201_README.md">`201 Index`</a>
<hr>

### <u>Array Methods</u>

##### Push Alternatives
- numArray[numArray.length] = 'newly pushed element';

##### Pop storing
- var last = numArray.pop();

##### Unshift / Shift
- numArray.unshift();
- var same = stringArray.shift(); - returns first element

### <u>String Methods</u>

##### Slice
- exampleString.slice(3, 15) - given index range
- exampleString.slice(15) - index 15 of a string and on

##### Split
- exampleString.split(' ');
- exampleString.split('', 6); - stops after a number of splits

##### Trim
- exampleString.trim(); - removes whitespace on either side of the string

### IIFE (immediately invoked function expression)
- (function fxName() { </br>
    console.log('start on load'); </br>
  })();

### Css Functions
- @keyframes name {</br>
}
- 'class or id' { </br>
  animation: name 20s infinite; </br>
}
