## Object Type
use ```typeof``` to get the type of a object
```
typeof 123; // 'number'
typeof NaN; // 'number'
typeof 'str'; // 'string'
typeof true; // 'boolean'
typeof undefined; // 'undefined'
typeof Math.abs; // 'function'
typeof null; // 'object'
typeof []; // 'object'
typeof {}; // 'object'
```
```null``` is object, ```Array``` is object

## Wrapper Object
Note:
1. Do ## NOT ## use ```new Number()、new Boolean()、new String()``` to create wrapper object
2. Use ```String``` to convert any type to string, or use ```toString()``` for a object
3. Do not need to convert any type to ```boolean```
4. ```typeof``` could get ```number、boolean、string、function and undefined```
5. Use ```Array.isArray(arr)```
6. Use ```myVar === null```

## Date
Create a date object:
```
var d = new Date(2015, 5, 19, 20, 15, 30, 123);
d; // Fri Jun 19 2015 20:15:30 GMT-0700 (Pacific Daylight Time)
```

## RegExp
https://www.regextester.com/
```
var re1 = /ABC\-001/
var re2 = new RegExp('ABC\\-001');
```
```
re.test('mock string'); // return true or false
```
1. Group: ```exec()```
2. Greedy match: ```?```
3. Global search: ```g```

## JSON (JavaScript Object Notation)
Data type:
 * number
 * boolean
 * string
 * null
 * array -- []
 * object -- { ... }
