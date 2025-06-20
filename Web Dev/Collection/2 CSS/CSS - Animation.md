```css
@keyframes myName {
	from {
		font-size: 10px;
		/* some properties */
	}
	
	to {
		font-size: 20px;
		/* some properties */
	}
}
```
- we can use `%` instead of `from` and `to` like:
	- `0%`
	- `50%`
	- `100%`
---
### Animation Properites
```css
animation-name: myAnimation;
animation-duration: 2s;
animation-timing-function: ease-in;
animation-delay: 1s;
animation-iteration-count: 3; /* infinite */
animation-direction: normal; /* reverse, alternate, alternate-reverse */

/* Short-hand */
animation: myName 2s linear 3s infinite normal;
```