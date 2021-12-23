# Section 2: Type Aias

### Definition
with the 'type' keyword
```
type combine = string | number;
type convertionDescriptor = 'as-number' | 'as-string'
```

### Advantage
This allows you to avoid unnecessary repetition and manage types centrally.

From
```
function greet(user: { name: string; age: number }) {
  console.log('Hi, I am ' + user.name);
}
 
function isOlder(user: { name: string; age: number }, checkAge: number) {
  return checkAge > user.age;

```

To
```
type User = { name: string; age: number };
 
function greet(user: User) {
  console.log('Hi, I am ' + user.name);
}
 
function isOlder(user: User, checkAge: number) {
  return checkAge > user.age;
}
```

