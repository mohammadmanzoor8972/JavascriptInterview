# JavascriptInterview
Javascript Interview Tricky Questions


## Reverse the case of character eg lower to upper.

Example : reverseUpper("HEllO woRLd");

```javascript
function reverseUpper(str){
     return str.split("").map(item=>item==item.toLowerCase() ? item.toUpperCase() : item.toLowerCase();
}
```

