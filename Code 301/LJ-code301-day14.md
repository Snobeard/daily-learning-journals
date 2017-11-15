# LJ Code 301 - Day 14
[`Home`](../README.md)
[`301 Index`](301_README.md)
<hr>

#### REGEX - replacing consecutive spaces with something else
- `(string).replace(/\s+/g, 'somethingElse');`

#### Distinguishing individual listeners
- `$('.recipes').on('click', 'a.show-more', function(...` *<- selects one*
</br> vs
</br> `$('a.show-more').click(function(...` *<-selects many*

#### Retrieve all branches
- `git pull origin` *<- fetches all branches from 'origin'*
