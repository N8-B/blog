## Coercing with Boolean, Number and String Objects in javascript
Today we are going to talk about this 3 global Objects(functions)  in Javascript and how to use them as **factory functions** to coerce differents values.   
##### Important:
- In javascript [functions are Objects](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md#values--types) too.

  ```javascript
  Function instanceof Object // true
  Boolean instanceof Function // true    
  Number instanceof Function // true    
  String instanceof Function // true    
  ```
- [Coersion](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md#coercion) is when a **conversion** from one type to another occur
- You need to understand de [differences between a factory function and a constructor function in JavaScript](https://medium.com/javascript-scene/javascript-factory-functions-vs-constructor-functions-vs-classes-2f22ceddf33e#.ogi8o4gs5) before keep reading.

## Using Boolean, Number and String as

### Constructor functions
If we use it with the `new` keyword then always **return an object**, not what we often want:

```javascript
var b = new Boolean(false); // { [[PrimitiveValue]]: false }
var n = new Number(10);     // { [[PrimitiveValue]]: 10 }
var s = new String('foo'); // { 0: "f", 1: "o", 2: "o", length: 3, [[PrimitiveValue]]: "foo" }
```

### Factory functions
When we use it as a factory function it will try to coerce the argument to the actual Type.

```javascript
var b = Boolean(false); // false
var n = Number(10);    // 10
var s = String("foo"); // "foo"
```

The interesting part is when we use it to coerce values to te desired type:

```javascript
var b = Boolean(""); // false
var b = Boolean(1); // true

var n = Number("10");    // 10
var n = Number("foo");   // NaN

var s = String(10); // "10"
```

### In an example
Get only the truthy values in an array

```javascript
var stuffs = ["", 1, undefined, { foo: "bar" }];
var validStuffs = stuffs.filter(Boolean); // [ 1, { foo: "bar" } ]
```
