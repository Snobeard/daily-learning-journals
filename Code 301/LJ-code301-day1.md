# LJ Code 301 - Day 1
<a href="../README.md">`Home`</a>
<a href="301_README.md">`301 Index`</a>
<hr>

#### 'Let' and 'Const'
- `let` is useful when using a variable only within it's given scope. </br>
ie: only use-able within it's loop / function

- `const` is useful when you have a variable or object that cannot be changed </br>
ie: `const drinkingAge = 21;` </br>
`drinkingAge = 16;` will not work because drinkingAge is a constant variable.

#### Template Literals
- first off..  <code>\`</code> (grave key) and not `'` (apostrophe)
- 'Hello there ' + name + '!' <br>
is the same as <br>
'Hello there ${name}!'

#### SMACCS (it's useful to organize css styling)
- General idea
  1. reset css
  2. base css - starter setup (general layout)
  3. layout css - more in depth organizing of style and design
  4. module css - fine detailing of specific components

#### Regular expressions - <a type="\_blank"  href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp">RegExp MDN</a>

- / <i>pattern</i> / <i>flags</i>
- `pattern = 'text of the regular expression'`
- `flags`
  1. `g` - global match, finds all matches instead of just the first
  2. `i` - ignore case
  3. `m` - multiline treat beginning `^` and end `$` characters as working over multiple lines
  4. `u` - unicode, treat pattern as a sequence of unicode code points
  5. `y` - sticky, matches only from the index indicated by `lastIndex` property
