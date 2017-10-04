# LJ Code 201 - Day 13

#### <u>Storage</u>

##### Persistence (server / cookies)
- reading server side data

##### localStorage
- .setItem('key', 'value')
- .getItem('key')
- .clear()
- localStorage.'key' = 'value'
- var stuff = localStorage.'key'

##### Persistence Layers
- Storage
  - Every time state is changed
    - every click
    - every 25 clicks
- retrieve
  - page load
  - if (localStorage exists) { <br>
    do stuff to local data - (assign what we retrive to a var or object)<br>
  } else { <br>
    do stuff to CREATE data - (create instances)<br>
  }
- clear
  - check if something works

#### JSON (JS Object Notation)
- JSON.stringify()
- JSON.parse()
