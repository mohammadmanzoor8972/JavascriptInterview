# JavascriptInterview
Javascript Interview Tricky Questions


## Reverse the case of character eg lower to upper.
Example : reverseUpper("HEllO woRLd");

```javascript
function reverseUpper(str){
     return str.split("").map(item=>item==item.toLowerCase() ? item.toUpperCase() : item.toLowerCase();
}
```

## Reverse the string without inbuild function
```javascript
function reverse(str){
let strs = "";
for(var x = str.length-1; x>0; x--){
strs+= str[x];
}
return strs;
}
```

## Get Duplication values from multip arrays.
Example : duplicate(..ar1, ...ar2, ...ar3)
```javascript
function dups(){
var obj = {};
var dupl = [];

if(arguments.length>0){
for(var index in arguments){
let arg = arguments[index]
for(var x=0; x<arg.length; x++){
if(!obj[arg[x]]){
obj[arg[x]] = arg[x]
} else {
dupl.push(arg[x])
}

}
}
}

return Object.values(obj);
}

```


