## Coercing with Boolean, Number and String objects in Javascript
![Goku transformation](https://raw.githubusercontent.com/juliomatcom/blog/master/content/goku-transform.gif)  
*Photo: [funnyjunk.com](http://funnyjunk.com/funny_gifs/4342692/best+friend+talking+to+my+crush)* 
  
Today we are going to talk about this 3 global Objects(functions)  in Javascript and how to use them as **factory functions** to coerce differents values.   
##### Important:
- In javascript [functions are Objects](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md#values--types) too. Boolean, Number and String are functions.

  ```javascript
  Function instanceof Object // true
  Boolean instanceof Function // true    
  Number instanceof Function // true    
  String instanceof Function // true    
  ```
- [Coersion](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md#coercion) is when a **conversion** from one type to another occur.
- You need to understand the [differences between a factory function and a constructor function in JavaScript](https://medium.com/javascript-scene/javascript-factory-functions-vs-constructor-functions-vs-classes-2f22ceddf33e#.ogi8o4gs5) before keep reading.

### Using Boolean, Number and String as:

#### Constructor functions (Bad)
If we use it with the `new` keyword then will always **return an object**, not what we expected:

```javascript
var b = new Boolean(false); // { [[PrimitiveValue]]: false }
var n = new Number(10);     // { [[PrimitiveValue]]: 10 }
var s = new String('foo'); // { 0: "f", 1: "o", 2: "o", length: 3, [[PrimitiveValue]]: "foo" }
```
This is a very confusing thing to do in your programs. All **3** are regular **objects** with prototype and methods. Don't use it.

#### Factory functions (Good)
When we use it as a factory function it will return the expected **type** value.

```javascript
var b = Boolean(false); // false
var n = Number(10);    // 10
var s = String("foo"); // "foo"
```

The interesting part is when we use it to perform a **type conversion**:

```javascript
var b = Boolean(""); // false
var b = Boolean(1); // true

var n = Number("10");    // 10
var n = Number("foo");   // NaN

var s = String(10); // "10"
```

### More examples

```javascript
var stuffs = ["", 1, undefined, { foo: "bar" }];
// Get only the truthy values inside stuffs
var onlyValids = stuffs.filter(Boolean); // [ 1, { foo: "bar" } ]
// Get only the numbers values inside stuffs (Note: 0 is falsy value so this won't work if 0 is in stuffs)
var onlyNumbers = stuffs.filter(Number); // [ 1 ]
```

Read more:
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String
