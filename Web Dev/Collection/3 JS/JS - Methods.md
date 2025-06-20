Actions that can be performed on an object.
```js
// Regular Method
const calculator = {
	add: function(a, b) {
		return a + b;
	}
	sub: function(a, b) {
		return a - b;
	}
}
```

```js
// Shorthand Method
const calculator = {
	add(a, b) {
		return a + b;
	}
	sub(a, b) {
		return a - b;
	}
}
```
---
```js
calculator.add(2, 3) // 5
calculator.sub(3, 2) // 1
```
---
## `this` Keyword
"`this`" is keyword refers to an object that is executing the current piece of code.
```js
const stu = {
	name: "Abhinav",
	age: 18,
	eng: 80,
	math: 79,
	hindi: 33,
	getAvg() {
		let avg = (this.eng + this.math + this.hindi) / 3;
		console.log(`Student ${this.name} got ${avg}%`);
		
		console.log(this); // to print whole object
	}
}
```
- We cannot access `eng`, `math`, `hindi` keys inside the object.
- To access we use `this` keyword.