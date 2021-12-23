# Section 2: Enum
Added by TS
A HUMAN readable way of values.
Use for limit the range of a variable

### Syntax
- JS way
    ```
    const PROCESSING = 1;
    const COMPLETED = 2;
    const HOLDED = 3;

    let statusList = ['completed', 'holded', 'processing'];
    let status = 'completed';
    let status2 = COMPLETED
    ```
- TS way
    ```
    // definition
    enum Status {PROCESSING, COMPLETED, HOLD} // default to 0,1,2
    or 
    enum Status {PROCESSING = 10, COMPLETED = 20, HOLD = 30} // can assign number or string values

    // usage
    status = Status.PROCESSING

    if (status === Status.PROCESSING) { ... ... }
    ```