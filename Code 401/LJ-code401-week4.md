# LJ Code 401 - Week 4
[`Home`](../README.md) [`401 Index`](401_README.md)
<hr>

#### Binary Tree
```
    1           / :  'left'  <edge>
   / \          \ :  'right'
  2   3         
     / \        node : 1-5
    4   5       depth : 1 = 0, 2|3 = 1, 4|5 = 2
                level : 1 = 1, 2|3 = 2, 4|5 = 3
                height : 1 = 2, 2 = 0, 3 = 1, 4|5 = 0
                leaf : <end-node> with no <left> or <right> (2,4,5)
                root : 1
```
```
Pre-Order: (root -> left -> right)
  1 -> 2 -> 3 -> 4 -> 5

Post-Order: (left -> right -> root)
  2 -> 4 -> 5 -> 3 -> 1

In-Order: (left -> root -> right)
  2 -> 1 -> 4 -> 3 -> 5
```

#### Binary Search Tree
```
(smaller) 10 (bigger)     bigO-worst : O(H) | O(n)
         /  \             bigO-Avg : O(H) | log(n)
        5   16            bigO-best : o(H) | log(n)
       / \   
      2   7 
```

#### K-ary Trees
```
          1                    bigO : O(n)
         / \   \   \   \
        2   3   7   8   9
           / \
          5  10

```
```
Breadth First : 1 -> 2 -> 3 -> 7 -> 8 -> 9 -> 5 -> 10
(Queue) levels first | Dijkstra | 
|1| + |2, 3, 7, 8, 9| + |5, 10|


Depth First : 1 -> 9 -> 8 -> 7 -> 3 -> 10 -> 5 -> 2
(Stack) leafs first
```

#### Basic Authorization
1. Account
    - Authorization
    - Password
2. Profile
    - Avatar 
    - Bio
    - Friends
3. Client
    - POST '/signup'
      - email
      - username
      - password
    - recieve `token`
        - long
        - unique
        - random
        - encrypted
4. Server
    - hash password
    - create `token seed` - (store in app)
    - unique random seed
    - encrypt - (send token user)
5. Authorization Header
    - Basic - username:password
    - Bearer <token>
6. GET request
    1. get /route
        - send id
        - set token
    2. server
        - bearer middleware
        - verify token
    3. profile router
        - find profile
    4. return error || 200 + json
7. POST request
    1. post /resource
        - content-type: multipart-form
    2. server
        - multer = multipart/form-data middleware
        - write to server hard drive
    3. AWS (amazon web service)
        - multer => receives key (filename)
        - send filename to client


###### Authentication
- able to authenticate `WHO` the user is

######  Authorization
- list of `ACTIONS` allowed to do

#### Hash Algorithm vs Crypto Algorithm
###### Hash
`'Gregor' => 1234...` (cannot go back)


###### Crypto
`'gregor' => 1234...`  .then  `1234... => 'gregor'`

#### AWS amazon web service
Bucket => file system
key => file name
access control list (ACL) => permissions
object = BLOB (binary large object)

#### Library vs SDK
- Library
    - meant for personal use and for others
- SDK
    - meant to be created for other users

#### Hash table - Heap
###### Hash table
- O(1)
- [ <array> ] => each index references a linked list

###### Heap
- no 'lookup' / used for showing either minimum or maximum
- Heap is an array 
- find children | 2(i) + 1(or)2 | for the index of the children
- values inserted on each level from left to right
- Min Heap
    - ascending values (starting at minimum numbers)
- Max Heap
    - descending values (starting at maximum numbers)
- Insertion
    - insert at last placeholder and bubble up, to replace parent value until happy
- Removal
    - smallest route -> remove the root, and bubble down starting with the last element

#### [Travis.ci.org](https://travis-ci.org)
- Continuous test integration for github project