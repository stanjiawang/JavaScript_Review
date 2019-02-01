use ```Object.create()``` instead of ```obj._proto_

Array object
```arr ----> **Array**.prototype ----> Object.prototype ----> null```

Function object
```foo ----> Function.prototype ----> Object.prototype ----> null```
