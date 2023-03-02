# 5.12 Getting index and value while looping: enumerate()

### Enumerate()

- A programmer commonly requires both the current position index and corresponding element value when iterating over a sequence.
- Example below demonstrates how using a for loop with range() and len() to iterate over a sequence generates a position index but requires extra code to retrieve a value:

![5%2012%20Getting%20index%20and%20value%20while%20looping%20enumera%20220884beb2a5457da08d6bda2cc13a0f/Untitled.png](5%2012%20Getting%20index%20and%20value%20while%20looping%20enumera%20220884beb2a5457da08d6bda2cc13a0f/Untitled.png)

- Similarly, a for loop that iterates over a container obtains the value directly, but must look up the index with a function call:

![5%2012%20Getting%20index%20and%20value%20while%20looping%20enumera%20220884beb2a5457da08d6bda2cc13a0f/Untitled%201.png](5%2012%20Getting%20index%20and%20value%20while%20looping%20enumera%20220884beb2a5457da08d6bda2cc13a0f/Untitled%201.png)

- The **enumerate()** function retrieves both the index and corresponding element value at the same time, providing a cleaner and more readable solution.

![5%2012%20Getting%20index%20and%20value%20while%20looping%20enumera%20220884beb2a5457da08d6bda2cc13a0f/Untitled%202.png](5%2012%20Getting%20index%20and%20value%20while%20looping%20enumera%20220884beb2a5457da08d6bda2cc13a0f/Untitled%202.png)

- The enumerate() function yields a new tuple each iteration of the loop, with the tuple containing the current index and corresponding element value.
    - In the example above, the for loop unpacks the tuple yielded by each iteration of enumerate(origins) into two new variables: "index" and "value".
- Unpacking is a process that performs multiple assignments at once, binding comma-separated names on the left to the elements of a sequence on the right.
    - Ex: num1, num2 = [350, 400] is equivalent to the statements num1 = 350 and num2 = 400.