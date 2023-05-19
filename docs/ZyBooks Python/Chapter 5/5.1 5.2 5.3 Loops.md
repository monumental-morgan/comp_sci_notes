# 5.1/2/3 Loops

- A **loop** is a program construct that repeatedly executes the loop's statements (known as the **loop body**) while the loop's expression is true; when false, execution proceeds past the loop
- Each time through a loop's statements is called an **iteration**.

### While loop basics

- **A while loop** is a construct that repeatedly executes an indented block of code (known as the **loop body**) as long as the loop's expression is True
    - At the end of the loop body, execution goes back to the while loop statement and the loop expression is evaluated again
- But, if the expression evaluates to False, then execution instead proceeds to below the loop body.

![5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled.png](5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled.png)

![5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%201.png](5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%201.png)

- **Sentinel value**: the value needed to terminate a loop

![5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%202.png](5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%202.png)

- **Good practice** is to include greater than or less than along with equality in a loop expression to help avoid infinite loops.

### Example: Greatest Common Divisor

![5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%203.png](5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%203.png)

### Example: Conversation

![5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%204.png](5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%204.png)

### Example: Getting input until a sentinel is seen

![5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%205.png](5%201%202%203%20Loops%20f95c026d77904d43b7dffa37a1a82245/Untitled%205.png)