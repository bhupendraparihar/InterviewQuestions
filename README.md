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
```javascript
typeof NaN
```

```css
/* use currentColor */
a {
  color: green;
}
a.office {
  color: blue;
}

/* instead of */
a:hover {
  border: 1px solid green;
}
a.office:hover {
  border: 1px solid blue;
}

/* use */
a:hover {
  border: 1px solid currentColor;
}
```

```javascript
(function(){
  return typeof arguments;
})();
```

```javascript
var f = function g(){ return 23; };
typeof g();
```

```javascript
(function(x){
  delete x;
  return x;
})(1);
```

```javascript
var y = 1, x = y = typeof x;
x;
y;
```

```javascript
(function f(f){
  return typeof f();
})(function(){ return 1; });
```

```javascript
var foo = {
  bar: function() { return this.baz; },
  baz: 1
};
(function(){
  return typeof arguments[0]();
})(foo.bar);
```

```javascript
var foo = {
  bar: function(){ return this.baz; },
  baz: 1
}
typeof (f = foo.bar)();
```

```javascript
var f = (function f(){ return "1"; }, function g(){ return 2; })();
typeof f;
```

```javascript
var x = 1;
if (function f(){}) {
  x += typeof f;
}
x;
```

```javascript
var x = [typeof x, typeof y][1];
typeof typeof x;
```

```javascript
(function(foo){
  return typeof foo.bar;
})({ foo: { bar: 1 } });
```

```javascript
(function f(){
 function f(){ return 1; }
 return f();
 function f(){ return 2; }
})();
```

```javascript
function f(){ return f; }
new f() instanceof f;
```

```javascript
with (function(x, undefined){}) length;
```
```javascript
var fruits = ['apple','orange'];

basket = fruits;

basket.push("mango");

console.log(fruits.length); //
console.log(basket.length);//
```
```javascript
var word = "Javascript";
var sentence = {
  construct:function( word ){
     return ?
  },
  word:"is"
};
console.log( sentence.construct("Awesome!") ); /// Javascript is Awesome! 
```

```javascript
var obj;

function foo(obj){
obj = {x:"world"};
}

obj = {x:"hello"};
foo(obj);

console.log(obj);//?
console.log(obj.x); //?
```

```javascript
var x = (function(){
  var temp = [];
  for (var i=0;i <= 10;i++){
    temp[i] = function (){
      return ( i ) * ( i + 1 ) / 2;
    }
  }
  return temp;
})();
console.log( typeof x[1] );//? 
console.log( x[3]() );//?? 
```

```javascript
var age = 101;
var father = {
  age: 98,
  getAgeOfSon: function() {
    var age = 40;
    this.age = 60;
    window.setTimeout(function(){
      console.log( this.age );
    }, 1000);
  }
}
father.getAgeOfSon();//? 101
```

```javascript
var dateOfBirth = 1985;

function getDateOfBirth(){
dateOfBirth = 2013;
return;

function dateOfBirth(){
return dateOfBirth;
}

}

getDateOfBirth();
console.log(dateOfBirth);


//console.log("Hello".display(5));
String.prototype.display = function(r){var repeatStr="";for (i=0;i<r;i++){repeatStr += this.toString()} return repeatStr;}
"hello".display(5)
```

```javascript
var dateOfBirth = getDateOfBirth();
function getDateOfBirth() {
  function dateofbirth(){}
  var dateofbirth
  
  return dateOfBirth; // undefined // 
  //  dateOfBirth = 1985;
    //function dateOfBirth() {}
    //var dateOfBirth = 2013;
}
console.log(typeof dateOfBirth);//?


(function(){
  var a = b = 3;
})();

console.log("a defined? " + (typeof a !== 'undefined'));
console.log("b defined? " + (typeof b !== 'undefined'));
```
