## Transitions

```css
/* 🎬 Transitions */
transition-duration: 1s;
transition-timing-function: ease-in;
transition-delay: 1s;

/* ✨ Shorthand */
transition: all 1s ease-in 1s;
/* Format: [property] [duration] [timing-function] [delay] */
```

---

### 🧲 `transform:`  
```css
transform: rotate(45deg);
transform: scale(1.5);
transform: translate(50px, 40px);
transform: translateX(50px);
transform: translateY(40px);
transform: skew(30deg);
```

- 🔄 `rotate(°)` → Rotates element  
- 🔍 `scale(n)` → Zoom in/out  
- 📦 `translate(x, y)` → Move in 2D space  
- ↔️ `translateX()` / ↕️ `translateY()` → Move along single axis  
- 📐 `skew(°)` → Slant the element

---

### 🌫️ `box-shadow:`  
```css
box-shadow: 10px 10px 15px rgba(0,0,0,0.3);
/* Format: [x-offset] [y-offset] [blur-radius] [color] */
```

---

### 🖼️ `background-image:`  
```css
background-image: url("https://google.com");
```

---

### 📏 `background-size:`
- `cover` → Fill and crop  
- `contain` → Fit completely, may leave space  
- `auto` → Stretch or default scale  

> 🧠 Pair with `background-repeat: no-repeat;` if needed.

---

## 📍 Positioning

```css
position: relative;
top: 10px;
right: 10px;
bottom: 0;
left: 0;
```

### Types of `position:`
1. `static` (📌 default)
2. `relative` (🔀 offset from normal position)
3. `absolute` (📍 relative to nearest positioned ancestor)
4. `fixed` (📌 sticks to screen)
5. `sticky` (like fixed)
### `z-index:` 
- `auto` (0) default
- `1`,  `2`  or `-3`