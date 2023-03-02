# 6.8 Functions are objects

- A function is also an object in Python, having a type, identity, and value.
- A function definition like def print_face(): creates a new function object with the name print_face bound to that object.
- A part of the value of a function object is compiled **bytecode** that represents the statements to be executed by the function
    - A bytecode is a low-level operation, such as adding, subtracting, or loading from memory
    
    ![The function adds 1 to an argument and returns the result. The corresponding bytecode for the function requires 4 bytecode operations to perform the addition, and 2 to return the result.](6%208%20Functions%20are%20objects%20d1e18fbc175e4688862687bdbcd5edda/Untitled.png)
    
    The function adds 1 to an argument and returns the result. The corresponding bytecode for the function requires 4 bytecode operations to perform the addition, and 2 to return the result.
    
- Functions can be passed like any other object as an argument to another function
- Consider the following example, which defines two different functions print_human_head() and print_monkey_head().
    - A third function print_figure() accepts a function as an argument, calling that function to print a head, and then printing a body.
    
    ![6%208%20Functions%20are%20objects%20d1e18fbc175e4688862687bdbcd5edda/Untitled%201.png](6%208%20Functions%20are%20objects%20d1e18fbc175e4688862687bdbcd5edda/Untitled%201.png)