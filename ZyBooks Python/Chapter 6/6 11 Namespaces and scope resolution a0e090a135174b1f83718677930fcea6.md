# 6.11 Namespaces and scope resolution

### Namespace

- A namespace maps names to objects.
- The Python interpreter uses namespaces to track all of the objects in a program
- In fact, a namespace is actually just a normal Python dictionary whose keys are the names and whose values are the objects
    - A programmer can examine the names in the current local and global namespace by using the locals() and globals() built-in functions.
    
    ![6%2011%20Namespaces%20and%20scope%20resolution%20a0e090a135174b1f83718677930fcea6/Untitled.png](6%2011%20Namespaces%20and%20scope%20resolution%20a0e090a135174b1f83718677930fcea6/Untitled.png)
    

### Scope and scope resolution

- Scope is the area of code where a name is visible.
- Namespaces are used to make scope work.
- Each scope, such as global scope or a local function scope, has its own namespace
- If a namespace contains a name at a specific location in the code, then that name is visible and a programmer can use it in an expression.

There are at least three nested scopes that are active at any point in a program's execution: 1

1. Built-in scope – Contains all of the built-in names of Python, such as `int()`, `str()`, `list()`, `range()`, etc.
2. Global scope – Contains all globally defined names outside of any functions.
3. Local scope – Usually refers to scope within the currently
executing function, but is the same as global scope if no function is
executing.
- When a name is referenced in code, the local scope's namespace is the first checked, followed by the global scope, and finally the built-in scope.
- If the name cannot be found in any namespace, the interpreter generates a NameError.
- The process of searching for a name in the available namespaces is called **scope resolution**.

### More scoping and namespaces

![Note that the Python Tutor tool uses the term "frame" in place of "namespace".](6%2011%20Namespaces%20and%20scope%20resolution%20a0e090a135174b1f83718677930fcea6/Untitled%201.png)

Note that the Python Tutor tool uses the term "frame" in place of "namespace".