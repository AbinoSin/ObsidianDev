## Variable Declarations

```js
var door = true;
let health = 89;
const maxHealth = 100;
```
```js
let a;             // ✅
let b = null;      // ✅
let c = undefined; // ❌ (same as: let a;)
```

> [!info] Identifier Rules
> - Can include: `letters`, `digits`, `_`, `$`
> - ❌ Cannot begin with a digit
> - Use ==camelCase== naming convention

---

## Data Types in JavaScript

### 1. Primitive Types

| Type        | Examples                                    |
| ----------- | ------------------------------------------- |
| `Number`    | `5`, `3.14`, `NaN`                          |
| `Boolean`   | `true` & `false`                            |
| `String`    | `"hello"`, `'world'`                        |
| `Undefined` | Variable declared but not assigned `let a;` |
| `Null`      | `null` (intentional) `let a = null;`        |
| `BigInt`    | `BigInt(123)` or `123n`                     |
| `Symbol`    | `Symbol("id")`                              |
>[!hint] ***NaN*** a number value
>The **NaN** global property is a value representing *"Not-a-Number"*
>```js
>0 / 0     // NaN
>NaN - 1   // NaN
>NaN * 1   // NaN
>NaN + NaN // NaN
>```

>[!hint] Difference between `null` and `undefined`
>```js
>let a;             // ❌ bad practice
>let a = undefined; // ❌ (same as above)
>let a = null;      // ✅ good practice
>```
>- `null` means **intentionally** not assign the value.
>- `undefined` no needs to assign, it automatically assigns if there is any need.
### 2. Non-Primitive Types

- `Object`
- `Array`
- `Function`
---
> [!tip] Use `typeof` to check the type:
> ```js
> typeof 123;       // "number"
> typeof "abc";     // "string"
> typeof true;      // "boolean"
> ```