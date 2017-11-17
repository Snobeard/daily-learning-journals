# LJ Code 301 - Day 15
[`Home`](../README.md)
[`301 Index`](301_README.md)
<hr>

#### CSS OverWriting
- When calling css later it has to be exactly the same.
- You can't style `#login .user` and then restyle the same features on `.user`
- it must be either `#login .user` = `#login .user`
</br> or `.user` = `.user`

#### Media scaling with jQuery
- `if ($(window).width() < 709) {` </br>
    `$('.main-nav ul').hide();` </br>
  `}`


#### Prevent click functionality (not recommended)
- `$('#login').click(function(event){` </br>
    `event.stopPropagation();` </br>
`});`
