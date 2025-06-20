## IF ELSE

```js
if (condition) {
  // do something
} else if (condition) {
  // do something
} else {
  // do something
}
```

> [!info] Use this structure for **step-by-step conditional checks**.

---

## Switch Statement

```js
let color = "red";

switch (color) {
  case "red":
    console.log("Stop");
    break;
  case "yellow":
    console.log("Wait");
    break;
  case "green":
    console.log("Go");
    break;
  default:
    console.log("Broken");
}
```

> [!tip] Best for **multiple exact matches** instead of chained `else if`.

---

## Ternary Operator

```js
condition ? exprIfTrue : exprIfFalse;
```
```js
age >= 18 ? "adult" : "not adult";
```

> [!example] One-line conditionals useful in simple logic assignments.
