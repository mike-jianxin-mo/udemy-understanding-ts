# Section 2: Unkown Type

### unknown vs any
- unknown is more strict than any
- unknown must work with dynamic type checking functions
  ```
    a: unkown;
    
    ... ...

    if (typeof a === 'string') {
        ... ...
    }
  ```