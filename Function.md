## defination
1. anonymous function
```function (x) { ... }```
2. ```arguments``` point to the parameter
3. ```rest```
```
function foo(a, b, ...rest) {
    console.log('a = ' + a);
    console.log('b = ' + b);
    console.log(rest);
}

foo(1, 2, 3, 4, 5);
// a = 1
// b = 2
// Array [ 3, 4, 5 ]

foo(1);
// a = 1
// b = undefined
// Array []
```
