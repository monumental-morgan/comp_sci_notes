# 6.6 Function Stubs

### Incremental development and function stubs

- Programs are typically written using **incremental development**
- To assist with the incremental development process, programmers commonly introduce **function stubs**, which are function definitions whose statements haven't been written yet.
- The benefit of a function stub is that the high-level behavior of the program can be captured before diving into details of each function
- Capturing high-level behavior first may lead to better-organized code, reduced development time, and even to code with fewer bugs.
- A programmer writing a function stub should consider whether or not calling the unwritten function is a valid operation.
    - One approach is to use the **pass keyword**, which performs no operation except to act as a placeholder for a required statement.

![The function steps_to_calories() above contains a single pass statement because at least one statement is required in any user-defined function](6%206%20Function%20Stubs%20cbad3aeb650f462c97b31057dd2ef09f/Untitled.png)

The function steps_to_calories() above contains a single pass statement because at least one statement is required in any user-defined function

![Another useful approach is to print a message when a function stub is called, thus alerting the user to the missing function statements.](6%206%20Function%20Stubs%20cbad3aeb650f462c97b31057dd2ef09f/Untitled%201.png)

Another useful approach is to print a message when a function stub is called, thus alerting the user to the missing function statements.

- Good practice is for a stub to return -1 for a function that will have a return value.
- In some cases, a programmer may want a program to stop executing if an unfinished function is called
    - Ex: A program that requires user input should not execute if the user-defined function that gets input is not completed.
    - In such cases, a **NotImplementedError** can be generated with the statement raise NotImplementedError
    - The NotImplementedError indicates that the function is not implemented and causes the program to stop execution

![6%206%20Function%20Stubs%20cbad3aeb650f462c97b31057dd2ef09f/Untitled%202.png](6%206%20Function%20Stubs%20cbad3aeb650f462c97b31057dd2ef09f/Untitled%202.png)