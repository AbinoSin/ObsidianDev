To see whole document:
```js
console.dir(document); // JS object with properties/methods
console.log(document); // HTML structure
```
```
text node
comment node
element node
```
---
## Selectors
>[!example] Query Selector
>Select anything like CSS
>```js
>document.querySelector("#myID / .myClass / tag")
>// returns first element
>```
>```js
>document.querySelectorAll(".myClass / tag")
>// returns a NodeList
>```
>- Returns **all** `<p>` elements (NodeList).

>[!done] By ID
>```js
>document.getElementById("myID")
>```

>[!done] By Class
>```js
>document.getElementsByClassName("myClass")
>```

>[!done] By Tag
>```js
>document.getElementsByTagName("div")
>```

>[!faq] By Attribute 
>```js
>node.getAttribute("attr")
>node.setAttribute("attrName", "value")
>```

>[!note] Style
>```js
>node.style
>```
---
## Navigation
-> `.parentNode` & `.parentElement`
-> `.childNodes` & `.children` (also `.children[0]`)

-> `.firstChild` & `.lastChild`
-> `.firstElementChild` & `.lastElementChild`

-> `.nextSibling` & `previousSibling`
-> `.nextElementSibling` & `.previousElementSibling`
