## 🌈 Colors & Backgrounds
```css
color: orange;                /* Named Color */
color: rgb(0, 99, 255);       /* RGB */
color: rgba(0, 99, 255, 0.5); /* RGB + Alpha */
color: #ff00ff;               /* HEX */
color: #f0f;                  /* Short HEX */
color: #ff00ff00;             /* HEX + Alpha */
color: transparent;
```
- `background-color:` works the same way!
- `opacity: 0.8;` sets **overall transparency** (not just color).

> 💡 **Alpha** only affects the color’s transparency.  
> 🧊 **Opacity** affects the entire element!

>[!hint]- There is also a `transparent` color value

---
## 📏 Units of Measurement

### 🔒 Absolute Units
- `px` → Pixels
- `pt` → Points (used in print)
- `pc` → Picas
- `cm`, `mm`, `in` → Physical length (rarely used on screen)
### 🔄 Relative Units
- `%` → Percentage (relative to parent)
- `em` → Relative to current font-size
- `rem` → Relative to root font-size
- `ch` → Width of "0" character
- `vh` → 1% of viewport height    
- `vw` → 1% of viewport width
---
## 📝 Text Alignment
```css
text-align: center;
```
- `left` / `start`
- `right` / `end`
- `center`
- `justify` — makes text edges line up on both sides
## ✍️ Text Decoration
```css
text-decoration: underline;
text-decoration: double blue underline;
```
- `none`, `underline`, `overline`, `line-through`
- Shorthand can include:
    - Line Style: `solid`, `dashed`, `double`
    - Color: any valid color
    - Thickness: `2px` etc.
## 🔠 Text Transform
```css
text-transform: uppercase;
```
- `none`, `uppercase`, `lowercase`, `capitalize`
---
## 🔤 Font Styling
```css
font-size: 16px;
font-family: 'Arial', sans-serif;
font-weight: bold;
```
### `font-weight:` Options:
- `normal` → 400
- `bold` → 700
- Numeric: `100` to `900`
- Relative: `bolder`, `lighter` (depends on parent)
---
## 📐 Line & Letter Spacing
```css
line-height: 2.5;
letter-spacing: 10px;
```
- `line-height:` Sets spacing between lines.
- `letter-spacing:` Adjusts space between characters.