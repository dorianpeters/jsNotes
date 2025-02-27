# Arrow Functions

Defined as "syntactically compact alternative" to a regular function expression.

```js
// Normal syntax
const square = (x) => {
    return x * x;
} 

const sum = (x, y) => {
    return x + x;
} 
```

All arrow function are anonymous functions, but they can be stored in a named variable.

The parens around the parameters are the beginning of the function and they are optional for one parameter, but needed for zero or two or more. . 

```js
// Normal syntax
const square = (x) => {
    return x * x;
} 

// parens needed due to zero parameters
const hello = () => {
    return "hello";
} 

// no parents needed due to one parameter
const square = x => {
    return x * x;
} 

// parens needed due to two paremeters
const sum = (x, y) => {
    return x + x;
} 
```

There are further situations where we don't need the curly braces and where we don't need the return statement. You can do an implicit return by replacing curly braces with parens or omitting the parens. It must end with an expression. 

```js
// Implicit return, no curly braces, but parens added.
const square = x => (
    x * x;  
) 

// Can remove curly braces and parents
const divide = (x, y) => x / y

// Must use parens around an implicit return of an object
const makeCard = () => ({suit: 'hearts', val: 3});

// Error: JS think's the curly braces are the beginning of a function
const makeCard = () => {suit: 'hearts', val: 3}; 
```


