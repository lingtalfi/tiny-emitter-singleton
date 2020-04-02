Tiny Emitter Singleton
===============
2020-04-02


A tiny emitter for web applications.

You can use it to make different modules communicate with each other via events.



Install
==========
```js
npm install tiny-emitter-singleton
```



Usage
=========

In script 1, do this:

```js
const ee = require('tiny-emitter-singleton');
ee.dispatch("removeBtnClicked", "any param", "any param2");
```

In script 2, do this:

```js
const ee = require('tiny-emitter-singleton');
ee.on("removeBtnClicked", (...args) => {
    console.log("removeBtnClicked", ...args);
});
```



Api
=======

- on (eventName, cb) 
- dispatch (eventName, ...args)







History Log
==========

- 1.0.0 -- 2020-04-02

    - initial commit