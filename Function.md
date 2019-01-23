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
2. apply ```function.apply(object, [array])``` // ```this``` bind to first parameter ```object```, ```array``` is function's parameters
3. call ```function.apply(object, parameter1, parameter2, ...)``` // ```this``` bind to first parameter ```object```, ```parameter1, parameter2, ...``` is function's parameters

## Higher-order function
1. map [“MapReduce: Simplified Data Processing on Large Clusters](https://ai.google/research/pubs/pub62)
```
'use strict';

function pow(x) {
    return x * x;
}
var arr = [1, 2, 3, 4, 5, 6, 7, 8, 9];
var results = arr.map(pow); // [1, 4, 9, 16, 25, 36, 49, 64, 81]
```
2. reduce 
```[x1, x2, x3, x4].reduce(f) = f(f(f(x1, x2), x3), x4)```
3. filter
4. sort
```
'use strict';
var arr = [10, 20, 1, 2];
arr.sort(function (x, y) {
    if (x < y) {
        return -1;
    }
    if (x > y) {
        return 1;
    }
    return 0;
});
console.log(arr); // [1, 2, 10, 20]
```

## closure
1. Returning Functions, return function instead of value, could get the value of this function only when you called it.
2. private variable
```
'use strict';

function create_counter(initial) {
    var x = initial || 0;
    return {
        inc: function () {
            x += 1;
            return x;
        }
    }
}
```

## arrow function
```this``` always point to lexical scope

## generator
```
function* foo(x) {
    yield x + 1;
    yield x + 2;
    return x + 3;
}
```
``` f.next```  ``` for ... of ```



