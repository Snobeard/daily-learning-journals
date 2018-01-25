# LJ Code 401 - Week 5
[`Home`](../README.md) [`401 Index`](401_README.md)
<hr>

#### Load Testing
1. Latency `20ms is good` </br>
   Time it takes for the user request to get to the api 
2. Processing Time </br>
   Time it takes for the server to process the request
3. Response Time </br>
   Time it takes for the server recieve the request, process the request, and send back the response

- RPS (requests per second) `1,000 is good`

- Performance `users we can support now`

- Scalability `users we can support eventually`

- Scenario </br>
  All the user actions


- Phase </br>
  different timestamps of heavy load

- Flow </br>
  specific actions the user makes

###### Artillery.js
1. Create `<name>.yml` file
2. `artillery run <name>.yml [-o ./<name>.json]`
3. `artillery report <name>.json`  

```
config:
  target: 'http://localhost:3000'
  phases:
    - duration: 5 # number of seconds
      arrivalRate: 20 # number of fake users per second
  processor: './load-test-create-user.js'
scenarios:
  - name: 'Create Users'
  - flow:
    - function: 'create'
    - post:
      url: '/signup'
      json:
        username: '{{username}}'
        email: '{{email}}'
        password: '{{password}}'
      capture:
        json: '$.token'
        as: 'token'
    - log: 'sent request for signup'
    - post:
      url: '/profiles'
      headers:
        Authorization: 'Bearer {{token}}'
      json:
        bio: {{bio}}
        avatar: {{avatar}}
    - log: 'sent request to profiles'
```

`load-test-create-user.js` -> create new users for each artillery user (export create function) 
```
(userContext, events, done) => {
  // add all fake variables for model creation
  userContext.vars.username = <fake name>
  userContext.vars.email = <fake email>
  userContext.vars.password = <fake password>
  userContext.vars.bio = <fake bio>
  userContext.vars.avatar = <fake avatar>
  
  return done();
}
```

#### [Webpack Concepts](https://webpack.js.org/concepts/)
1. Entry </br>
   imports all the dependencies from one file traversing the dependency tree
2. Output </br>
   bundle.js -- simplified output from the entry
3. Loaders </br>
   converts valid matches into modules
4. Plugins </br>
   sets up the configuration to do anything

###### node packages
- webpack
- webpack-dev-server
- html-webpack-plugin
- extract-text-webpack-plugin
- node-sass
- sass-loader
- resolve-url-loader
- css-loader
- babel-core
- babel-loader
- babel-preset-react
- babel-preset-es2015 (babel-preset-env)
- babel-plugin-transform-object-rest-spread
- react
- react-dom

#### React

###### Member Functions
methods you create for each react Component

###### Hooks
methods that react auto runs for you
ex: render()

###### State
- State
database state

- UI State

- V state
view state

#### Redux

Provider
  - holds store
Store
  - used to store all application's state
    - getState()
    - dispatch() - change state
    - subscribe()
Reducer (middleman - takes in state, and an action. Returns new state from the store)
  - defines app state
  - defines interations to app store
  (action)
    - type: 'string'
    - payload: <anything>
      - item_create | cat_update

#### React/Redux Definitions
<dl>
  <dt>React</dt>
  <dd>component based javascript library for building UI</dd>

  <dt>Dispatch</dt>
  <dd>dispatches actions to a reducer to change the store</dd>

  <dt>Store</dt>
  <dd>stores all the state in the application</dd>

  <dt>State</dt>
  <dd>all the information we store in the application and use to interact with the user</dd>

  <dt>Reducer</dt>
  <dd>fn(state, action) => new state</dd>

  <dt>Action</dt>
  <dd>{ type, payload } -> dispatch an action into the reducer to update the store</dd>

  <dt>Payload</dt>
  <dd>defines what values are changed in the state</dd>

  <dt>Redux</dt>
  <dd>a library used to manage the state in the application</dd>

  <dt>Provider</dt>
  <dd>used to store the 'Store' - react-redux</dd>
</dl>