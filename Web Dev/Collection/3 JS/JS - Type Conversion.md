## Implicit (Type Coercion)

> [!example] JavaScript auto-converts types:
> ```js
> '5' + 2       // "52"     → 2 becomes string
> '5' - 2       // 3        → '5' becomes number
> true + 1      // 2        → true becomes 1
> ```

> [!warning] `+` triggers string concatenation if **either operand** is a string.

---

## Explicit Type Conversion

#### To String
```js
String(123);          // "123"
(123).toString();     // "123"
true.toString();      // "true"
```

#### To Number
```js
Number("123");        // 123
parseInt("123.45");   // 123
parseFloat("123.45"); // 123.45
+"123";               // 123
```

#### To Boolean
```js
Boolean(1);           // true
Boolean(0);           // false
Boolean("");          // false
Boolean("hi");        // true
```

#### To BigInt
```js
let num = BigInt(3 ** 53);
```

---

## ⚠️ Falsy Values in JS

> [!danger] These evaluate to `false` in Boolean context:
> - `0`
> - `""` (empty string)
> - `null`
> - `undefined`
> - `NaN`
> - `false`
