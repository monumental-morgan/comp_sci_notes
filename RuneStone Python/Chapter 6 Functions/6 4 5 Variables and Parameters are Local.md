# 6.4/5 Variables and Parameters are Local

- An assignment statement in a function creates a **local variable**
- It is called local because this variable only exists inside the function and you cannot use it outside.
- it is legal for a function to access a global variable. However, this is considered **bad form** by nearly all programmers and should be avoided.
- Local Variables
    - Python looks at the variables that are defined as local variables in the function. We call this the **local scope**
- Global Variables
    - If the variable name is not found in the local scope, then Python looks at the global variables, or **global scope**

# 6.5 The Accumulator Pattern

- This pattern of iterating the updating of a variable is commonly referred to as the **accumulator pattern**
- We refer to the variable as the **accumulator**
- Remember that the key to making it work successfully is to be sure to initialize the variable before you start the iteration.
- Once inside the iteration, it is required that you update the accumulator.

### Main use case

```python
initialize the accumulator variable
repeat:
    modify the accumulator variable

# when the loop terminates the accumulator has the correct value
```