# LJ Code 301 - Day 12
[`Home`](../README.md)
[`301 Index`](301_README.md)
<hr>

#### API request Authorization
```
$.ajax({
  url: 'https://api.github.com/user/repos?type',
  method: 'GET',
  headers: {
	Authorization: 'token 336acd70a4dd7f81087edb407df664ded7af1a11' },
})
.then(data => console.log(data))
```
#### API Non-Authorization
```
$.get('https://api.github.com/users/snobeard/repos')
.then(data => console.log(data))
```

#### [Open Graph Protocol](http://ogp.me/)
- `<meta property="og:image" content="http://example.com/ogp.jpg" />`


- `og:image` - Identical to og:image.
- `og:image:secure_url` - An alternate url to use if the webpage requires HTTPS.
- `og:image:type` - A MIME type for this image.
- `og:image:width` - The number of pixels wide.
- `og:image:height` - The number of pixels high.
- `og:image:alt` - A description of what is in the image (not a caption). If the page specifies an og:image it should
