# Null

Doing typeof on a variable assigned to `null` will return `"object"` instead of `"null"`.

```javascript
var a = null
typeof a //"object"
```

This is a known problem with javascript but changing it would cause so many bugs that it will likely never be changed. 

# Function

```javascript
function foo() {
  return "hello"
}

typeof foo() //"string"
```
