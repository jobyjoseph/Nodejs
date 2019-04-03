## What is Nodejs?

It is an open source, cross-platform, run-time environment for JavaScript.

## Working of Nodejs

Nodejs is built on top of V8 engine. Node is just another C++ program written on top of V8 C++ code. When we run `node app.js`, app.js file is passed to the C++ program which in turn execute it using V8 engine.

Nodejs is single threaded. That means, a single thread is used to serve all clients.

Nodejs is asynchronous. So it can handle lot of clients. But, do not execute big CPU intensive jobs like video encoding, image manipulation and so on in node.

## Global vs Window object
Just like `window` object in browser, Nodejs have `global` object, which have global methods like `console`, `setTimeout` etc.

There is a small difference between them wrt to variable declaration.

In a browser, following code outputs 5.
```javascript
var a = 5;
console.log(window.a); // 5
```
But in Nodejs, similar approach gives `undefined`.
```javascript
var a = 5;
console.log(global.a); // undefined
```
The reason, is the variable is not automatically attached to `global` object.
