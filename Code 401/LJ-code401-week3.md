# LJ Code 401 - Week 3
[`Home`](../README.md) [`401 Index`](401_README.md)
<hr>

#### Binary Search Tree - log2

#### Doubly Linked List
```
{ value: 7,
  previous: null,
  next : { value: 8
           previous: { value:7, previous:null <loop...>}
           next: { value: value: 9
                   previous: { value:8, previous:{ value:7, previous:null <loop...>} <loop...>}
                   next: null
                 }
         }
  }
```

#### Object-Relational Mapping (ORM)
- Mongoose
- Security
- Ease of access

#### Databases
- Oracle
- MongoDB
- CouchDB
- SQL Server
- Postgres

##### PostGres vs Mongo
- Postgres
  - Relational Database
  - Organized tables
- Mongo
  - NoSQL Database
  - collection of files

#### Mongoose
```
Person.find({})
.where('name.last').equals('Ghost')
.limmit(10)
.sort('-occupation')
.select('name occupation')
.exec(callback)
```

IMPORT INFO 
```
`mongoimport --jsonArray --db nowmusic --collection tracks now-thats-what-i-call-music.json` </br>
 mongoimport <--jsonArray> --db <database name> --collection <collection name> <pathtofile>
```