# LJ Code 201 - Day 16
<a href="../README.md">`Home`</a>
<a href="201_README.md">`201 Index`</a>
<hr>

#### Arrays (sorting)
- a = array[0]
- b = array[0 + 1]
- points.sort(function(a, b){return(a - b)}); - returns ascending integers
- points.sort(function(a, b){return(b - a)}); - returns descending integers
- points.sort(function(a, b){return 0.5 - Math.random()}); - random order
- cars.sort(function(a, b){return a.year - b.year}); - sorting by object properties
- cars.sort(function(a, b){  - sort string properties </br>
   var x = a.type.toLowerCase(); </br>
   var y = b.type.toLowerCase(); </br>
   if (x < y) {return -1;} </br>
   if (x > y) {return 1;} </br>
   return 0; </br>
});
