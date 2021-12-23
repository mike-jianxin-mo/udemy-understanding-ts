# Section 2: Function return type

### void Vs undefined

1. In JS, undefined is the return value of a function without return or empty return.

2. In TypeScript, the void is a function without return. undefined is a function with an empty return.

### Example
Which code snippet is better (i.e. which code should you write)?
1)
```
function sayHi(): void {
  // ...
}
```
OR

2)
```
function sayHi(): undefined {
  // ...
}
```
1) because it doesn't force you to return anything if you don't want to return something