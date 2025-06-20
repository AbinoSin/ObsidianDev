## **1 - `for` Loop**
The `for` loop in JavaScript is a **basic and powerful loop** used to repeat a block of code a specific number of times. It gives you **full control** over the loop: when it starts, when it ends, and how it progresses.

>[!danger] Syntax
>```js
>for (initialization; condition; update) {
>	// code block to execute
>}
>```
- `initialization`: Run once before the loop starts (usually used to declare a counter).
- `condition`: Checked before every loop iteration. If `true`, the loop runs.
- `update`: Runs after each iteration (usually used to update the counter).

>[!example]- Example: Counting 1 to 5
>```js
>for (let i = 1; i <= 5; i++) {
>	console.log(i);
>}
>```
>```js
>1
>2
>3
>4
>5
>```

---
## **2 - `while` Loop**
A `while` loop repeats a block of code **as long as a given condition is `true`**. It checks the condition **before** each iteration.
>[!danger] Syntax
>```js
>while (condition) {
>	// code block to run
>}
>```

>[!example]- Example: Print numbers 1 to 5
>```js
>let i = 1;
>while (i <= 5) {
>	console.log(i);
>	i++;
>}
>```
>```
>1
>2
>3
>4
>5
>```

---
## **3 - `do...while` Loop**
A `do...while` loop is **similar to a while loop**, but with one key difference:
> ✅ It runs the block **at least once**, even if the condition is false.

>[!danger] Syntax
>```js
>do {
>	// code block to run
>} while (condition);
>```

---
## **4 - `for...of` Loop**
The `for...of` loop in JavaScript is used to **iterate over iterable objects**, such as arrays, strings, maps, sets, etc. It provides a clean and simple syntax to loop through the **values** of an iterable (not the indexes/keys).

**Mostly used for:**
- ==Strings==
- ==Arrays==
- not recommended for objects

>[!danger] Syntax
>```js
>for (const item of iterable) {
>	// code block to execute
>}
>```
>- NOTE: `item` will store the value of index, not index no.

>[!example]- Example with Set
>```js
>const numbers = new Set([1, 2, 3, 2]);
>
>for (const num of numbers) {
>	console.log(num);
>}
>```
>```js
>1
>2
>3
>```

>[!example]- Example with Array
>```js
>const fruits = ['apple', 'banana', 'mango'];
>
>for (const fruit of fruits) {
>	console.log(fruit);
>}
>```
>```
>apple
>banana
>mango
>```

>[!example]- Example with a String
>```js
>const name = "Abhinav";
>
>for (const char of name) {
>	console.log(char);
>}
>```
>```
>A
>b
>h
>i
>n
>a
>v
>```

---
## **5 - `for...in` Loop**
The `for...in` loop in JavaScript is used to **iterate over the enumerable properties (keys)** of an object (or the indexes of an array). It's most useful when working with **objects**, not arrays.
>[!danger] Syntax
>```js
>for (const key in object) {
>	// code block to execute
>}
>```

>[!example]- Example with an Object
>```js
>const person = {
>	name: "Abhinav",
>	age: 18,
>	city: "Surat"
>};
>
>for (const key in person) {
>	console.log(key, person[key])
>}
>```
>```
>name Abhinav
>age 18
>city Surat
>```

>[!example]- Example with an Array
>```js
>const colors = ['red', 'green', 'blue'];
>
>for (const index in colors) {
>	console.log(index, colors[index]);
>}
>```
>```
>0 red
>1 green
>2 blue
>```
>- ⚠️ *Only for* ***Arrays,*** `for...in` gives the **index**, not the value. So it's not ideal for arrays (use `for...of` instead for values).

---
>[!important] Use of `break` Keyword
>The `break` statement in JavaScript is used to **exit a loop early,** immediately stopping the execution of that block.

>[!example] Example in FOR LOOP
>```js
>for (let i = 1; i <= 10; i++) {
>	if (i === 5) {
>		break;
>	}
>}
>```