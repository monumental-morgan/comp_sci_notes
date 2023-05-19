# 5.4 Counting

### Counting up with a while loop

- The programmer can use a variable to count the number of iterations, called a loop variable

![5%204%20Counting%20336b686ea5724cdf8f0be47e4f50632f/Untitled.png](5%204%20Counting%20336b686ea5724cdf8f0be47e4f50632f/Untitled.png)

- **A common error** is to forget to include the loop variable update (e.g., i = i +1) at the end of the loop, causing an unintended infinite loop.

### Counting down with a while loop

- The loop body executes when i is 5, 4, 3, 2, and 1, but does not execute when i reaches 0.

![5%204%20Counting%20336b686ea5724cdf8f0be47e4f50632f/Untitled%201.png](5%204%20Counting%20336b686ea5724cdf8f0be47e4f50632f/Untitled%201.png)

![5%204%20Counting%20336b686ea5724cdf8f0be47e4f50632f/Untitled%202.png](5%204%20Counting%20336b686ea5724cdf8f0be47e4f50632f/Untitled%202.png)

### Shorthand operators

- Covered in [2.5/6/7](https://www.notion.so/2-5-6-7-Expressions-e642db5cc91848659453b017354ac310)
- The item on the right can be an expression, so num *= x + y is shorthand for num = num * (x + y)