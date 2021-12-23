# Section 2: Core Types

#### Type checking
```
if (typeof n1 === 'number') { ... ... }

throw new Error('type error!')

```

#### Type types
- Dynamic type: JS uses.
  type can be changed during runtime

- Static type: TypeScript Uses
  type can not be changed.

#### Always lowercases
<strong>The core primitive types in TypeScript are all lowercase!</strong>

In TypeScript, you work with types like string or number all the times.

Important: It is string and number (etc.), NOT String, Number etc.


#### Even with TS, there is still chances to yield type errors with JS
4:50
a ``` string + number ``` error

#### definition type
Not a good practise, type could be inferred
```
let n1: number = 5;
```

A good practise
```
let n1: number;
n1 = 50;
```

# Words
- infer
- inference