## Definition
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

## Scope
1. global object ```window```
2. local scope, use ```let``` instead of ```var```
3. naming space, bind variables and function to a unique global variable
4. constants， ```const```

## Destructuring assignment

## Object method
1. ```this``` point to current object
2. apply ```function.apply(object, [array])``` // ```this``` bind to first parameter ```object```, ```array``` is function's parameter

