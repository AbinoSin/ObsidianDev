```js
setTimeout(function, timeout);  // run one time
setInterval(function, timeout); // runs multiple time
```
- In `timeouot` we enter time in mili seconds. (1000 = 1s)
---
## ID for set interval
```js
let someID = setInterval(() => {
	console.log("Hello");
}, 1000);
```
Now if we print the `someID` it will print `1` which is the iD of this `setInterval`

---
To stop this we use
```js
clearInterval(someID); // name of the vaiable
```