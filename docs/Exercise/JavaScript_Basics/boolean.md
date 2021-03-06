## Excercise to understand 'Boolean' data type

### What are boolean data types?

JavaScript **Boolean** is a data type which can store any one of two values, **true** or **false**.
E.g. - 

```
// Javascript has a specific constructor for creating Boolean type objects
const testValue = new Boolean(true);

console.log(testValue);    // it prints **Boolean {true}** since testValue is an Object of type Boolean
```

We can directly assign boolean value to any variable, like below:

```
const isTrue = true;
const isfalse = false;
```

In JavaScript, a **truthy** value is a value that translates to true when evaluated in a Boolean context. 
All values are truthy unless they are defined as **falsy**.

Javascript treats an empty string (**""**), **0**, **undefined** **null** and **NaN** as **falsy**.

Not operator or **!** is the operator which is used to **negate** the boolean aspect of a value.

For example:
```
const val = 12;

// using ! operator
console.log( !false );   // prints true
console.log( !12 );      // prints false, since 12 is truthy value and negation of a truthy value is falsy

// using !! operator - this returns just the boolean context of any value
console.log( !!true );   // prints true
console.log( !!false );  // prints false
console.log( !!12 );     // prints true, since 12 is truthy value and negation of a truthy value is falsy, and again negation of that false value is truthy

```

Let us go through some more examples below to understand the concepts:

```
console.log( !!0 );            // false

console.log( !!1 );            // true

console.log( !!undefined );    // false

console.log( !!null );         // false

const emptyString = '';

console.log( !emptyString );   // true
console.log( !!emptyString );  // false

const anyString = "test value";

console.log( !anyString );     // false
console.log( !!anyString );    // true

const obj = {};

console.log( !obj );           // false
console.log( !!obj );          // true

const arr = [];

console.log( !arr );           // false
console.log( !!arr );          // true

const negativeNum = -1;

console.log( !negativeNum );    // false
console.log( !!negativeNum );   // true

```
