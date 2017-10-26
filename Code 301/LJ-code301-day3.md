# LJ Code 301 - Day 3
<a href="../README.md">`Home`</a>
<a href="301_README.md">`301 Index`</a>
<hr>

#### <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">RegExp</a> (patterns used to match character combinations in strings)
- Expression Literal
  - `/ab+c/g`
- Constructor Function
  - `new RegExp('ab+c', 'g')`
- `[abc]` - match precisely what you want (a|b|c)
- `\` - selects special character
- `^` - matches beginning of input (followed by selections)
- `$` - matches end of input
- `*` - matches the preceeding expression 0 or more times (`/bo*/` = `'b'` | `'booooo'`
- `+` - matches the preceeding expression 1 or more times (`/a+/`) = `'a'` | `'aaaaaa'`
- `?` - matches the preceeding expression 0 or 1 time (`/e?le?/`) = `'el'` | `'le'` | `'l'`
- `.` - matches any single character (`/.n/`) = `'on'` | `'an'`, <p style="display: inline; color:#ff3300; font-weight: bold;">EXCEPT:</p> `'near'`
- `/(x)/` - matches x and remembers for later use. Called in the same instance with `\1` `\2` etc.. and called later, or in a .replace() method perhaps with `$1` `$2` etc..
