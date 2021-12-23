# Section2: Tuples
Added by TS

### Definition
No tuple type in JS/TS. 
Tuple is an array of the same length & type.
Using Union Type to achieve it.
```
role = [2, 'author']
(string | number) []
```
To get more explicity, specify the detial type of a Tuple. 
```
role: [number, string]
```

** Note:
But the PUSH function cann't be checked by TS
The following will pass TS checking.
```
role.push('admin')
```
So we have to use assignment, because TS will check assignment!
```
role = [10, 'test']
```