
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
**Note** Cannot use ```.```, use ```A['high-school']``` ```// 'P A High'```
