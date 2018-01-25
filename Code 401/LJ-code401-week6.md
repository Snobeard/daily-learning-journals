# LJ Code 401 - Week 6
[`Home`](../README.md) [`401 Index`](401_README.md)
<hr>

#### SCSS
###### `@import 'filename'` will import the `_filename.scss` file

###### @include | [@mixins](https://scotch.io/tutorials/how-to-use-sass-mixins)
```
------------------------------------
@mixin myMixin($variable) {
  border: $variable;
  padding: $variable;
  box-sizing: border-box; 
}
------------------------------------
$five = 5px;

@import myMixin($five);

```

#### Webpack
###### Debug Development
environment plugin
define plugin - define constants, (ex: `__API_URL__`)
`uglifyjs-webpack-plugin`
`clean-webpack-plugin`

###### Production
webpack-clean - create a new build each time
webpack-uglifier - reduce file size by limiting variable names and others

#### Cookies
__browser commands__
`document.cookie` => string of all cookies
`document.cookie.split(';')` => array of all the cookies
`document.cookie.split(';').map(cookie => cookie.split('='));` => array of key value pairs