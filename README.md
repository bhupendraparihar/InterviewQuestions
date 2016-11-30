# InterviewQuestions
My favorite list of Programming Interview Questions

```javascript
function a(x) { return x*2; }
var a;
alert(a);
```

```javascript
function b(x, y, a) {
  arguments[2] = 10;
  alert(a);
}
b(1, 2, 3);
```

```javascript
function a() {
  alert(this);
}
a.call(null);
```

```javascript
if (!("a" in window)) {
  var a = 1;
}
alert(a);
```

```javascript
var a = 1,
  b = function a(x) {
    x && a(--x);
  };
alert(a);
```

```javascript
var a = function b() {
  return "Hi World";
};
typeof(b());
```

```javascript
var github;
github == undefined;
```

```javascript
(function(){
  return typeof arguments;
})();
```

```javascript
(function(x){
  delete x;
  var a = x;
  return a;
})('github');
```

```javascript
var x = 0;
alert(x === false);
```

```javascript
undefined = 'Hello World';
var github;
github == undefined;
```

```javascript
var x = 0;
alert(x == false);
```

```javascript
0.1 + 0.2 == 0.3
```

```javascript
null instanseof Object
```

```javascript
typeof null
```
