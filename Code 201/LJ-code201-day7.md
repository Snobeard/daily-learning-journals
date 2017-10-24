# LJ Code 201 - Day 7
<a href="../README.md">`Home`</a>
<a href="201_README.md">`201 Index`</a>
<hr>

### Object Literals
var myObject = {</br>
&nbsp;&nbsp;  key: value, </br>
&nbsp;&nbsp;  key: value, </br>
&nbsp;&nbsp;  key: function() {} </br>
};

### Constructor Functions
function MyObject () { </br>
&nbsp;&nbsp;  this.key = value; </br>
&nbsp;&nbsp;  this.key = value; </br>
};
###### Prototype
Object.prototype.name = function() { </br>
parameters </br>
};

### Table
 - < table > - initiate table
 - < th > - table header
 - < tr > - table row
 - < td > - table data

 - console.table(parameter) - displays as a table

### Creating DOM Elements
  1. create the element  -- document.createElement('li');
  2. give it content -- .textContent = 'content here';
  3. append it </br>-- document.getElementById('id here') </br>
       -\- .appendChild(element);
