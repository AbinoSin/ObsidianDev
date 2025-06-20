## Enabling Flex
```css
display: flex;
display: inline-flex;
```
---
### Warp
```css
flex-wrap: nowrap;     /* Default – all items stay on one line */
flex-wrap: wrap;       /* Items will wrap onto multiple lines if needed */
flex-wrap: wrap-reverse; /* Same as wrap, but in reverse direction */
```
---
### Direction
```css
flex-direction: row; /* ➡️ (default) */
flex-direction: row-reverse; /* ⬅️ */
flex-direction: column; /* ⬇️ */
flex-direction: column-reverse; /* ⬆️ */
```
---
### Main Axis Alignment
```css
justify-content: flex-start; /* default */
justify-content: center;
justify-content: flex-end;
justify-content: space-between;
justify-content: space-around;
justify-content: space-evenly;
```
---
### Cross Axis Alignment
```css
align-items: stretch;       /* default */
align-items: flex-start;
align-items: center;
align-items: flex-end;
align-items: baseline;

align-content: stretch;
align-content: flex-start;
align-content: center;
align-content: flex-end;
align-content: space-between;
align-content: space-around; /* default */
```
---
### Gaps
```css
row-gap:      
column-gap:
gap:           /* Short-hand */
```

---
### Item Control 
**Use these properties in display flex child items**
```css
align-self:       /* overrides `align-items` per item */
order:            /* controls item order */

flex-grow:        /* (default 0) — controls how much an item grows */


flex-shrink:      /* (default 1) — controls how much it shrinks */
flex-shrink: 0;   /* This will prevent item to shrink */

flex-basis:       /* (default auto) — initial size before growing/shrinking */
flex-basis: 0;    /* This will make the item as shrinked as possible */

flex: [grow] [shrink] [basis]  /* shorthand */
```
---

>[!faq] `place-content:` is short-hand for `justify-content` and `align-content`

>[!hint] `gap` property add gap between items