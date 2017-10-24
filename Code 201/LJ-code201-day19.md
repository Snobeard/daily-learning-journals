# LJ Code 201 - Day 19
<a href="../README.md">`Home`</a>
<a href="201_README.md">`201 Index`</a>
<hr>

#### Splicing Strings (return partial string)
- function myFunction() { </br>
    var string = "Some text you want to end here. ...but it keeps going."; </br>
    var result = string.slice(0, 31); </br>
} </br>
returns ('Some text you want to end here.')

- var result2 = string.slice(5, -10); </br>
returns ('text you want to end here. ...but it ke')
