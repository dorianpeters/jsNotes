# Reduce function

Reduce runs a "reducer" function on every element in an array, resulting in a _single value_. 
It executes a callback on each element, passing in the value returned by the *previous execution*.
```js

// Find sum of array
nums.reduce((sum, currentVal) => {
    return sum + currentVal;
}, 0);

// Find max number in array
nums.reduce((max, currentVal) => {
    if (currentVal > max) return currentVal;
    return max;
});

