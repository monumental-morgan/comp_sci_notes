# 4.9 Membership and identity operators

### Membership operators: in/not in

- Determining whether a specific value can be found within a container, such as a list or dictionary
- The **in** and **not in** **operators**, known as membership operators, yield True or False if the left operand matches the value of some element in the right operand, which is always a container.

![4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled.png](4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled.png)

![4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled%201.png](4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled%201.png)

- Membership operators can be used to check whether a string is a **substring**, or matching subset of characters, of a larger string.
    - Example, 'abc' in '123abcd' returns True because the substring abc exists in the larger string.

![4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled%202.png](4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled%202.png)

- Finding membership in a dictionary only applies to the key, NOT the value

Example:

![4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled%203.png](4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled%203.png)

### Identity operators: is/is not

- The programmer can use the identity operator, **is**, to check whether two operands are bound to a single object.
- The inverse identity operator, **is not**, gives the negated value of 'is'. Thus, if x is y is True, then x is not y is False.

![4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled%204.png](4%209%20Membership%20and%20identity%20operators%20e7887c6b9d58497aa9e3f64abb3c9dbe/Untitled%204.png)