# JavaScript Tips and Tricks 01

JavaScript Tips and Tricks

### Question 01

```javascript
log(null == undefined);
Ans: True;
log(null === undefined);
Ans: False;
```

### What is IIFE

`IIFE (Immediately Invoked Function)`

```javascript
(function () {
  log("Hello IIFE");
})();
```

### Array.prototype.flat()

`The flat() method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.`
`EX: flat()
flat(depth)`

```javascript
const arr1 = [1, 2, 3, [4, 5]];
log(arr1.flat());
//output: [0, 1, 2, 3, 4]
const arr2 = [1, 2, 3, [[[4, 5]]]];
log(arr2.flat(2));
//output: [0, 1, 2, [3, 4]]
```
