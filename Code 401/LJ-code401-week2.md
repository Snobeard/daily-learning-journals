# LJ Code 401 - Week 2
[`Home`](../README.md) [`401 Index`](401_README.md)
<hr>

#### Little Endian -vs- Big Endian
- os.endianness()
- little endian - reads from right to left (most computers)
- big endian - reads from left to right (androids, etc..)

#### image file formats
- BMP - [Wiki](https://en.wikipedia.org/wiki/BMP_file_format)

#### Big O
- Basic Operations (super quick)
  - `+`
  - `-`
  - `===`
  - `*`
  - `/`
  - `()`
- GOOD
  - constant ( `+, -, *, /, =, ===, ()` )
  - lgn  ( `binary search tree` )
  - nlgn ( `.sort` )
  - linear ( `for loop` )
- BAD
  - quadratic
  - cubed ()
  - exponential ( `nested loops` ) 
  - factorial ( 3! )

#### Linked Lists
- algorythms(data)
- array = [4, 3, 2, 1, 8]
  - find => `O( n )`
  - array[1] => `O( 1 )`
  - insert => `O ( n )`
  - remove => `O( n )`
- linked list - []=>[]=>[]=>[]
  - find => `O( n )`
  - list[5] => `O( n )`
  - insert => `O( 1 )`
  - remove => `O( 1 )`

#### README documentation - [beginners guide](https://medium.com/@meakaakka/a-beginners-guide-to-writing-a-kickass-readme-7ac01da88ab3)
- must be able to look at the readme and understand what it does
  - project title
  - features
  - examples
  - tests
    - make sure `npm install` installs jest
    - `npm run test`
  - how to use
  - credits!
  - sources

#### OSI model - [wiki](https://en.wikipedia.org/wiki/OSI_model)
- 

#### Winston - [docs](https://www.npmjs.com/package/winston)
- log severity
  - 0       Emergency: system is unusable
  - 1       Alert: action must be taken immediately
  - 2       Critical: critical conditions
  - 3       Error: error conditions
  - 4       Warning: warning conditions
  - 5       Notice: normal but significant condition
  - 6       Informational: informational messages
  - 7       Debug: debug-level messages
