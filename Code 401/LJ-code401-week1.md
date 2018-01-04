# LJ Code 401 - Week 1
[`Home`](../README.md) [`401 Index`](401_README.md)
<hr>

#### View File in Terminal Window
- `cat <filename>`

#### [Error Syntax's](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)
- [EvalError](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/EvalError)
- [InternalError](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/InternalError)
- [RangeError](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RangeError)
- [ReferenceError](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/ReferenceError)
- [SyntaxError](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/SyntaxError)
- [TypeError](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/TypeError)
- [URIError](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/URIError)

####  try - catch - finally
- `try` tests functions
- `catch` happens if there is an error
- `finally` always occurs

#### call - bind - apply (historical `new`)
- `call` Array.prototype.reduce.call(arguments, ...
- `bind`
- `apply`

#### `jest -i --coverage --watch`
- `-i` waits for each test to process
- `--coverage` shows table at bottom of test process containing lines covered and %'s
- `--watch` continously cycles tests as you update the files

#### `exceptions` vs `-1`
- `exceptions` cannot be ignored
- `-1` can be ignored

#### Interviewing Process
1. Re-state the problem
2. Work through an example
  - Test for edge cases
    - null/undefined
    - empty
    - duplicated values
    - incorrect types
    - mixture of data types
  - assumptions
3. Think about implementation
  - pseudo-code
4. Write code
5. Test the code with `correct input` and `edge cases`
  - step by step process
