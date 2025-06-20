>[!done]
>```js
>// Searching
>cars.indexOf("bmw");         // Returns index or -1 if not found
>cars.includes("limozen");    // Returns true or false
>```
>```js
>// Sorting
>cars.sort(); // Sorts alphabetically (doesn’t work well with numbers)
>```
>---
>```js
>// Other useful methods
>cars.concate(bikes);  // Merge two arrays (does NOT modify original)
>cars.toString();      // Make the array into string (does NOT modify original)
>cars.reverse();       // Reverse the array
>```
>---
>```js
>// Slicing
>cars.slice(startIdx, endIdx); // Extracts part (does NOT modify original)
>cars.slice(startIdx);         // Extracts to the end
>	// endIdx is optional and inclusive
>```

>[!done] `.splice(startIdx, deleteCount, newEl1, newEl2, ...)`
>- Changes in Original
>- `startIdx` Where to start?
>- `deleteCount` How many delete from start?
>- `newEl1, ...` What add to start?
>```js
>let numbers = [1, 2, 3, 4, 5, 6, 7];
>```
>```js
>// Add element '101' on the 2 index
>numbers.splice(2, 0, 101);         // 1, 2, 101, 3, 4, 5, 6, 7
>
>// Delete element 101
>numbers.splice(2, 1);              // 1, 2, 3, 4, 5, 6, 7
>
>// Replace element '3' to '101'
>numbers.splice(2, 1, 101);         // 1, 2, 101, 4, 5, 6, 7
>```
>```js
>// This will act as ".slice()"
>numbers.splice(3);                 // 1, 2, 3
>```

---
## **forEach**
It allows you to run a function for **each element** of the array.
```js
array.forEach(function(currentValue, index, array) {
  // Your code here
});
```
- `currentValue` → The current item in the array.
- `index` (optional) → The index (position) of the current item.
- `array` (optional) → The entire array itself.

>[!example]-
>```js
>let fruits = ["apple", "banana", "cherry"];
>
>fruits.forEach(function(fruit, index) {
>  console.log(index + ": " + fruit);
>});
>```
>```
>0: apple
>1: banana
>2: cherry
>```
### Key points:

- It **loops** through every element.
    
- It **cannot be stopped or broken** like a `for` loop (`break` or `return` won't stop it).
    
- It’s **used for performing actions**, not for transforming arrays. (For transforming, we use `.map()`.)
---
## **Map** Loop in Arrays
It **transforms** each element of the array and creates a **new array** with the results.
```js
let newArray = array.map(function(currentValue, index, array) {
  // return new value here
});
```

---
## **Filter**
Creates a new array of elements that gives true for a condition/filter.
```js
let newArray = array.filter(function(currentValue, index, array) {
  return condition;
});
```
- If the condition returns `true`, the item is kept.
- If `false`, the item is skipped.

>[!important] **In `.filter()`, the function should return a boolean**, so simply:
>```js
>const filteredNumbers = numbers.filter((currentValue) => {
  return currentValue % 2 === 0;
});
>```
>or
>```js
>const filteredNumbers = numbers.filter(num => num % 2 === 0)
>```
>This if the current value's operation is true than the value used 
---
## **Reduce**
Used to **reduce** an array to a **single value**.

**This value could be:**
- a number (sum, product, etc.)
    
- a string
    
- an object
    
- even a completely new array
```js
let result = array.reduce(function(accumulator, currentValue, index, array) {
  return newAccumulatorValue;
}, initialValue);
```
- `accumulator` → carries over the result
    
- `currentValue` → current item in the array
    
- `initialValue` → starting value of accumulator

>[!example]-
>```js
>let numbers = [1, 2, 3, 4, 5];
>
>let sum = numbers.reduce(function(accumulator, currentValue) {
>  return accumulator + currentValue;
>}, 0);
>
>console.log(sum);
>```
>```
>15
>```

### ✅ Key points:

- `.reduce()` always returns **one single value**.
    
- Very powerful for things like:
    
    - totals
        
    - averages
        
    - max/min
        
    - flatten arrays
        
    - counting items
        
    - building objects