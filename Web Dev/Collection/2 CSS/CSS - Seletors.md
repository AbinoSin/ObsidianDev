1. **Universal** Selector: `*`
2. **Elements** Selector: `h1`
3. **ID** Selector: `#myID`
4. **Class** Selector: `.myClass`
---
**Attribute Selector**
Eg - Selects all radio button
```css
input[type="radio"] {}
```

**Descendant Selector**
Eg - Selects all paragraphs inside divs
```css
div p {}
```

**Adjacent Sibling Combinator**
Eg - H3 that comes immediately after paragraph
```css
p + h3 {}
```

**Child Combinator**
Eg - Selects all buttons which are direct children of spans
```css
span > button {}
```

---
#### Pseudo Class
1. `:hover`
2. `:active`
3. `:checked`
4. `:nth-of-type()`

#### Pseudo Elements
1. `::selection`
2. `::first-letter`
3. `::first-line`

```css
selector:pseudoCode {
	/* do something */
}
```

`this is inline code`

```language-name
this is code block
```