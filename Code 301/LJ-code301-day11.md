# LJ Code 301 - Day 11
[`Home`](../README.md)
[`301 Index`](301_README.md)
<hr>

#### Event Handlers
- turns out you can duplicate event handlers.
- If you have an initPage method that invokes the event handlers, then you happen to use that method again, It will add another instance to the event so that it loops through consecutively each time the method is called.
