# LJ Code 401 - Week 5
[`Home`](../README.md) [`401 Index`](401_README.md)
<hr>

#### Load Testing
1. Latency `20ms is good`
  - Time it takes for the user request to get to the api </br>
2. Processing Time
  - Time it takes for the server to process the request </br>
3. Response Time
  - Time it takes for the server recieve the request, process the request, and send back the response

- RPS (requests per second) `1,000 is good`
  - 

- Performance `users we can support now`

- Scalability `users we can support eventually`

- Scenario
  - All the user actions


- Phase
  - different timestamps of heavy load

- Flow
  - specific actions the user makes

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
