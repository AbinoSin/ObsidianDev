## Syntax
```js
const post = {
username: "@CoderAbino",
likes: 78,
tags: ["@abino", "@ashsis", "@vivek", "@bittu"]
};
```
- Key will automatically converted into string

## To Access
```js
// First method
post["username"];  // '@CoderAbino'
post[variable];    // '@CoderAbino' (variable stores "username")

// Second method
post.username;     // '@CoderAbino'
```
```js
post.likes += 1;
```
## To add / update values
```js
post.username = "@xyz";  // update
post.dislike = 13;       // add (if not exsist)
```
```js
delete post.dislike;     // delete
```
## Others
```js
objt.keyValue.nestedKeyValue  // nested keyvlaue
arry[0].keyValue              // object in array

```
- JS automatically converts objects keys to strings (even if we made the number as a key, the will be converted to string)