# 6.12 Function Arguments

### Function arguments and mutability

- Arguments to functions are passed by object reference, a concept known in Python as **pass-by-assignment.**
- When a function is called, new local variables are created in the function's local namespace by binding the names in the parameter list to the passed arguments.

![6%2012%20Function%20Arguments%2044d83cf0520c44a49c85201cc5461e63/Untitled.png](6%2012%20Function%20Arguments%2044d83cf0520c44a49c85201cc5461e63/Untitled.png)

- When a function modifies a parameter, whether or not that modification is seen outside the scope of the function depends on the *mutability* of the argument object.
- If the object is **immutable**, such as a string or integer, then the modification is limited to inside the function. Any modification to an immutable object results in the creation of a object in the function's local scope, thus leaving the original argument object unchanged.
- If the object is **mutable**, then in-place modification of the object can be seen outside the scope of the function. Any operation like adding elements to a container or sorting a list that is performed within a function will also affect any other variables in the program that reference the same object.

![6%2012%20Function%20Arguments%2044d83cf0520c44a49c85201cc5461e63/Untitled%201.png](6%2012%20Function%20Arguments%2044d83cf0520c44a49c85201cc5461e63/Untitled%201.png)

- Sometimes a programmer needs to pass a mutable object to a function but wants to make sure that the function does not modify the object at all.

![One method to avoid unwanted changes is to pass a copy of the object as the argument instead, like in the statement my_func(num_list[:])](6%2012%20Function%20Arguments%2044d83cf0520c44a49c85201cc5461e63/Untitled%202.png)

One method to avoid unwanted changes is to pass a copy of the object as the argument instead, like in the statement my_func(num_list[:])