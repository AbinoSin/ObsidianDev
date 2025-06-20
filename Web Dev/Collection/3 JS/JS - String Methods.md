>[!danger] Strings are ==**_immutable_**==
---
```js
str.toUpperCase()
str.toLowerCase()
```
---
```js
str.trim()
```
- Removes *whitespaces* from start and end
---
```js
str.slice(star, end)
```
- Returns part of string
- `end` is optional
- `end` is non inclusive
---
```js
str.concat(str2)
```
- Joins `str2` with `str1`
- Same as (str1 + str2)
---
```js
str.replace("searchVal", "newVal")
str.replaceAll()
```
```js
str.repeat()
```
---
```js
str.charAt(idx)
```
- Find character on given index number
---
```js
str.indexOf("love")
```
- Returns first occurrence in string
- Or give `-1` if not found