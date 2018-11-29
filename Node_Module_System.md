When we declare a new variable or function in browser JavaScript, it is attached to global `window` object. But such a binding does not happen in Nodejs. In Nodejs, each variable or function is restricted to that particular file. That is how Node module system works.

### Hoisting in Nodejs
Inside a file, hoisting works inside Nodejs.
```javascript
console.log(a); // undefined
var a = 6;
```
