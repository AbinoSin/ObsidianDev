### Enabling Grid
```css
display: grid;
display: inline-grid;
```
---
### Defining Columns & Rows
```css
grid-template-columns: 1fr 30%; /* two equal columns */
grid-template-rows: auto 100px; /* one auto-height row, one fixed */
```
- `repeat(n, value)` — e.g. `repeat(3, 1fr)` for 3 equal columns
- `minmax(min, max)` — e.g. `minmax(200px, 1fr)`

---
### Gap Between Items
```css
gap: 20px; /* sets both row and column gaps */
row-gap: 10px;
column-gap: 15px;
```
---
### Placing Items
```css
grid-column: 1 / 3; /* spans columns 1 to 3 */
grid-row: 2 / span 4; /* spans rows 2 to 4 */
```
---
- `grid-column-start` / `grid-column-end`
- `grid-row-start` / `grid-row-end`
---
### Aligning Content
- `justify-items` and `justify-self` — align items horizontally (start, end, center, stretch)
- `align-items` and `align-self` — align items vertically (start, end, center, stretch)
- `place-items` and `place-self`
---
- `justify-content` — align whole grid horizontally
- `align-content` — align whole grid vertically
---
### Grid Areas (Optional)
- `grid-template-areas`
- `grid-area: header` — place item in a named area
