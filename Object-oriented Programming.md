use ```Object.create()``` instead of ```obj._proto_

Array object
```arr ----> Array.prototype ----> Object.prototype ----> null```

Function object
```foo ----> Function.prototype ----> Object.prototype ----> null```

## Constructor
Note: Capitalize the first letter of the function.
```
function Student(name) {
    this.name = name;
    this.hello = function () {
        alert('Hello, ' + this.name + '!');
    }
}
```
```
var xiaoming = new Student('Xiaoming');
xiaoming.name; // 'Xiaoming'
xiaoming.hello(); // Hello, Xiaoming!
```
```xiaoming ----> Student.prototype ----> Object.prototype ----> null```
```
function Student(name) {
    this.name = name;
}

Student.prototype.hello = function () {
    alert('Hello, ' + this.name + '!');
};
```

## Prototypal inheritance
```
function inherits(Child, Parent) {
    var F = function () {};
    F.prototype = Parent.prototype;
    Child.prototype = new F();
    Child.prototype.constructor = Child;
}
```

## class inheritance
```
class Student {
    constructor(name) {
        this.name = name;
    }

    hello() {
        alert('Hello, ' + this.name + '!');
    }
}
```
```
var xiaoming = new Student('小明');
xiaoming.hello();
```
```
class PrimaryStudent extends Student {
    constructor(name, grade) {
        super(name);
        this.grade = grade;
    }

    myGrade() {
        alert('I am at grade ' + this.grade);
    }
}
```
