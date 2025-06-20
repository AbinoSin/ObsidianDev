## Output
```js
console.log("Hello");                        // Normal output
console.error("Someting wrong");             // Error msg in red color
console.warn("This is a warning");           // Waring msg in yellow color
```
```js
alert("waring");                             // For Pop-up
```
```js
console.dir(window.document); // Specialy for objects
```
---
## Input
```js
prompt("Enter Your Roll No:");               // For input with popup
```
```js
let name = prompt("Enter Your Name:");       // for input in variable
```
---
>[!bug] 1 - Template Literals
>```js
>`Your pay ${a + b} rupees`
>```
>- `${a}` is String interpolation.
>- Can be used in any sitution.

>[!bug] 2 - Evaluates Multiple Expressions
>```js
>"Your pay", a + b, "rupees"
>```
>- Mostly use in print on console.

>[!bug] 3 - Concatenation
>```js
>"Your pay " + (a + b) + " rupees"
>```
>- Mostly use in variable declaration.

>[!bug] Escape Characters
>```js
>\n     // for new line
>\t     // for tab space
>```
>- For escape characters the `.length` property count it as only 1 character even its 2 or more character.