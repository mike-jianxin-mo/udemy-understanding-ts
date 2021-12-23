# Section 2: never type

### never vs void

The never type is better than void type, although it is inferred as void type.

But it can avoid the code errors caused by the throw function.

### User cases
- Throw
  ```
    function a():void/never {
        throw ...
    }
    // error!, if using void, but never can avoid it.
    console.log(a())
  ```
- Infinite loop 
  ```
    while() {}
  ```