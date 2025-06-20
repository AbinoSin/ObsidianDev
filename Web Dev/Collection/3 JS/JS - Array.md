>[!summary]- Theory
>- Arrays are **ordered**, **mutable**, and **zero-indexed** collections.
>- Can store **multiple values** of any type (including other arrays and objects).
>---
>- Arrays are **linear collections** of items
>	- Think of arrays as a single horizontal line of boxes: `|0|1|2|3|`
>	- **Index (position)** matters — unlike keys in objects.
>---
>- Arrays are a type of **object** in JavaScript.
>- Useful for **storing lists**, **iterating**, and **performing bulk operations**.

>[!danger] Arrays are ==**_mutable_**==

---
>[!danger] Syntax
>```js
>// 📦 Creating Arrays
>const arr1 = [1, 2, 3];          // Numeric array (Constant array)
>const arr2 = ["a", "b", "c"];    // String array 
>let arr3 = [1, "a", true, null]; // Mixed types
>let arr4 = [];                   // Empty array
>var nested = [[1, 2], [3, 4]];   // Nested (2D) array
>```
>```js
>// 🎯 Accessing Elements
>arr3[1]               // "a"
>nested[1][0]          // "3" (3rd character of "water")
>```
>```js
>// 🔄 Modifying Elements
>arr1[1] = 99;            // changes second item to 99
>arr1[arr1.length] = 100; // adds to end
>```

---
>[!done] Modifying
>```js
>let cars = ["audi", "bmw"];
>```
>```js
>// ( + ) Adding elements
>cars.unshift("maruti");   // Add to start
>cars.push("toyota");      // Add to end
>```
>```js
>// ( - ) Removing elements
>cars.shift();             // Remove start and return
>cars.pop();               // Remove end and return
>```
>```js
>// How they return?
>let delItem = cars.pop(); // Store deleted item
>```