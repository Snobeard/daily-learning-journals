# LJ Code 301 - Day 13
[`Home`](../README.md)
[`301 Index`](301_README.md)
<hr>

#### Handlebars - Filling a Data Array as Individual Components

###### Template
- `{ingredients: [onion, tomato, carrot, celery]`
- `{{#ingredients}}` - opening
- `<li>{{this}}</li>` - each array
- `{{/ingredients}}` - closing


###### OutPut
- `<li>onion</li>`
- `<li>tomato</li>`
- `<li>carrot</li>`
- `<li>celery</li>`
