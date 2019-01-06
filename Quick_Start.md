
# Basic grammer

1. automatically add ```;``` at the end
2. comment ```//```  or ```/* ... */```


# Data types and variables
1. ```isNaN(NaN); // true```
2. ```2 / 0; // Infinity```
3. ```0 / 0; // NaN```
4. ```1 / 3 === (1 - 2 / 3); // false```
5.  0 is a number, '' means empty string, null is empty value

# String
1. multiple lines string could use ``` `...` ```
2. ```var message = `Hi, ${name}, you are ${age} year old this year.` ```
3. ```toUpperCase```, ```toLowerCase```, ```indexOf```, ```substring``` will **NOT** change the original string

# Array
1. ```indexOf```, ```slice```, ```push```, ```pop```, ```unshift```, ```shift```, ```sort```, ```reverse```, ```splice```, ```contac```, ```join``` will **NOT** change the original string

# Object
1. use ```''``` if property name contain special character.
```
var A = {
  name: 'mock name',
  birthday: '01\/01\/2019',
  height: 6,
  'high-school': 'P A High'
}
```
**Note**: Cannot use ```A.high-school```, use ```A['high-school']``` ```// 'P A High'```
2. ```hasOwnProperty()``` to decide whether the this prop is owned by the object itself.

# Condition

# Loop

# Map & Set
1. Set only has keys, keys could not be same

# iterable
1. ```for ... of```
```
var s = new Set(['A', 'B', 'C']);
for (var x of s) {
    console.log(x);
}
```
```
var s = new Set(['A', 'B', 'C']);
s.forEach(function (element, sameElement, set) {
    console.log(element);
});
```
```
var m = new Map([[1, 'x'], [2, 'y'], [3, 'z']]);
m.forEach(function (value, key, map) {
    console.log(value);
});
```
```
var a = ['A', 'B', 'C'];
a.forEach(function (element) {
    console.log(element);
});
```

