>[!success] Linking JS in document
>```html
><script src="app.js"></script>
>```
>- Add this line of code before `</body>` tag.
>- So it can load after the whole document.

>[!summary] Things to know
>- `.js` is the file extension.
>- `// not exacutable` Comments.

>[!faq] Higher order functions
>A function who takes others functions as parameter or returning any function.

>[!summary] Theory
>>[!faq] Truthy & Falsy Value
>>- Everything in JS is true or false (in boolean context)
>>- This does't mean their value itself is false or true, but they are treated as false or true if taken in boolean context.
>>- **Falsy Value**: False, 0, -0, On (Bigint value), "" (empty string), null, undefined, NaN
>>- **Truthy Value**: Everything else
>1. JS is dynamic language and TS is static.
>2. Strings are immutable in JavaScript
>3. **Scope** determines the *accessibility* of variables, objects, and functions from different parts of the code.
>	- **Global Scope** - We can use it anywhere.
>	- **Function Scope** - Variables defined inside a function are not accessible (visible) from outside the function.
>	- **Block** - Variables declared inside a `{}` block cannot be accessed from outside the block.
>	- **Lexical** - A variable defined outside a function can be accessible inside another function defined after the variable declaration. The opposite is not true
>4. Hoisting

- 🔍 **Fun fact:** `typeof null` returns `"object"` — this is a known **quirk in JavaScript** (a bug from early JS days that's never been fixed due to backward compatibility).
