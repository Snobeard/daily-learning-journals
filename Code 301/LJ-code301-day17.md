# LJ Code 301 - Day 17
[`Home`](../README.md)
[`301 Index`](301_README.md)
<hr>

#### Click everywhere besides where you choose
- `$('html').click(function(e) {` </br>
  `if (!$(e.target).data('login')) {` </br>
    `$('#login').slideUp();` </br>
  `}` </br>
`});`
