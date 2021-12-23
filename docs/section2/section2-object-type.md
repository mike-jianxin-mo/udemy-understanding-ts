# Section 2: Object Type

#### Example
* Note: 
  - the semicolon;
  - has nested object definition.
```
const person: {
    name: string;
    age: number;
} = {
    name: 'Mike',
    age: 50
}
```

#### Object Type Vs Object
- The object type is similar to object, ONLY difference is object type is key-type pair, while objects are key-value pair.
- The generic object type CAN NOT be used for type checking.
  It can not even recognise the defined item in an object.
- Type will be removed in the compiled JS codes.

#### Generic Type: object
```
const person: object = {... ...}
```
{} is the same as object
```
const person: {} = {... ...}
```

