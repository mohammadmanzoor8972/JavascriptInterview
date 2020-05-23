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

## Reverse the array without inbuild function
```javascript
function reverseArrayInPlace(arr) {
  for (var i = 0; i <= Math.floor((arr.length - 1) / 2); i++) {
      let el = arr[i];
      arr[i] = arr[arr.length - 1 - i];
      arr[arr.length - 1 - i] = el;
  }
  return arr;
}
```


## Find Duplicate values from multiple arrays.
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

return Object.values(dupl);
}

```

## Find Palindrome String
```javascript
Example : "HelloWorld" => false
"HelloolleH" => true

function isPalindrome (str){
return str.split("").reverse().join("")==str
}
```

## Find Consecutive Character
```javascript
function letterCount(str){
  var s= str.match(/([a-zA-Z])\1*/g)||[];
return s.map(function(itm){
  return [itm.charAt(0), itm.length];
});
}
```



