# LJ Code 301 - Day 6
<a href="../README.md">`Home`</a>
<a href="301_README.md">`301 Index`</a>
<hr>

#### REST (Representational State Transfer)
- create => Post
- read => Get
- update => Put
- delete => delete

#### CRUD (Create Read Update Delete)

#### AJAX
`$.ajax({
  url: 'https://pokeapi.co/api/v2/pokemon/1',
  method: 'GET',
  success: function(data, messsage, xhr) {
    console.log(data);
  },
  fail: function(err) {
    console.error(err);
  }
})`
