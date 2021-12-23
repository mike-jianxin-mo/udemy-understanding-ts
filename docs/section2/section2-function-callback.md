# Section 2: Callback function

### Definition
```
function addAndHandle(n1: number, n2: number, cb: (num: number) => void) {
    const result = n1+ n2;
    cb(result)
}
```

### The function return: void
The void is used to flag whether the return value will be useful.
It would be find to have a return in the callback function when the return of the callback function definition is void.
I think this is for the complicated running environment of callback functions. 
One call backfunction may be applied in different places, sometime needs the return value, sometimes don't. So it is better for the callbackfunction definition to ignore the return in it.

### Examples:
- Function return 
    That's correct. As you learned, callback functions can return something, even if the argument on which they're passed does NOT expect a returned value.
    ```
    function sendRequest(data: string, cb: (response: any) => void) {
    // ... sending a request with "data"
    return cb({data: 'Hi there!'});
    }
    
    sendRequest('Send this!', (response) => { 
    console.log(response);
    return true;
    });
    ```

