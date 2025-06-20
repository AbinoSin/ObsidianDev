The `try` statement allows you to define a block of code to be tested for errors while it is being executed.

The `catch` statement allows you to define a block of code to be executed, if an error occurs in the try block.

>[!note] In simple words
>After an error the code stops working from the point of error execute.
>This `try` and `catch` statement prevents the error to from stopping the code of execution after the error
>- The key point is, you already need to predict that this line of code could become error.

```js
try {
	console.log(a);
} catch {
	console.log("variable 'a' not exsist");
}
```

```js
try {
	console.log(a);
} catch(err) {
	console.log(err); // this will show what's the error
}
```