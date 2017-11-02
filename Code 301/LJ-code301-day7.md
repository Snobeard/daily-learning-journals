# LJ Code 301 - Day 7
<a href="../README.md">`Home`</a>
<a href="301_README.md">`301 Index`</a>
<hr>

#### Set Time Interval (for functions)
- `window.setInterval('function()', 'time');`

#### [ExpressJS](http://expressjs.com/en/4x/api.html)
- Load the express library from node_modules </br>
`const express = require('express');`

- Instantiate express so we can use its functionality </br>
`const app = express();`

- Designate a port to serve our app on </br>
"process" is in the Node environment, use a port if it is set up, or set your own </br>
`const PORT = '4005'; // process.env.PORT`

- Tell the server which directory to serve files from </br>
`app.use(express.static('./public'));`

- Set up a route to send a message </br>
`app.get('/sam', function(request, response) {` </br>
`console.log('This will show up in Node');` </br>
`response.send('This will show up in Browser');` </br>
`});`

- Set up a route to send a file </br>
`app.get('/demi', function(request, response) {` </br>
`console.log('demi page loaded');` </br>
`response.sendFile('demi.html', {root: './public'});` </br>
  // res.sendFile('./public/demi.html', {root: '.'}); </br>
`})`

- error 404 </br>
`app.get('/\*', function(request, response) {` </br>
`res.send('This ain\'t sam or demi');` </br>
`})`

- Can we perform other methods on the same route? </br>
`app.post('/demi', callback);`

- Start the app so it listens for changes </br>
`app.listen(PORT, function() {` </br>
`console.log('listening on ${PORT}'');` </br>
`})`
