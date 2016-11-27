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
