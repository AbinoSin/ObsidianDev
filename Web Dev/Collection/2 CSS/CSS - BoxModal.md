
## 📐 Box Model Properties

### Dimensions
```css
/* normal */
height:
width:

/* minimum */
min-height:
min-width:

/* maximum */
max-height:
max-width:
```

### Spacing
```css
padding:
margin:
```

### Borders
```css
border:
border-radius:
```

---

## 🎨 Border

Shorthand syntax: `border: [width] [style] [color];`
### Individual Properties
- `border-width:`
- `border-style:`
	- `none`
	- `hidden`
	- `solid`
	- `dotted`
	- `dashed`
	- `double`
	- `groove`
	- `ridge`
	- `inset`
	- `outset`
- `border-color:`
### Border Sides
```css
border-top:
border-right:
border-bottom:
border-left:
border-bottom-color: /* or any other specific side + property */
```
---
## 🌀 Border Radius
- `border-radius:` — Rounds the corners.
    - `15px` → standard curve
    - `50%` → full circle (for square elements)
#### Individual Corners
```css
border-top-right-radius: 5px;
border-top-left-radius: 5px;
border-bottom-right-radius: 5px;
border-bottom-left-radius: 5px;
```
---
## 📦 Padding (Margin also same)
Controls inner space between content and border.

**Individual Sides**
```css
padding-top: 10px;
padding-bottom: 10px;
padding-left: 10px;
padding-right: 10px;
```

**Shorthand Forms**
```css
padding: 10px;                  /* All Sides */
padding: 10px 20px;             /* Top & Bottom | Left & Right */
padding: 10px 20px 30px;        /* Top | Left & Right | Bottom */
padding: 10px 20px 30px 40px;   /* Top | Right | Bottom | Left */
```