# 5.8 Nested Loops

- A **nested loop** is a loop that appears as part of the body of another loop
- The nested loops are commonly referred to as the outer loop and inner loop.
- Nested loops have various uses. One use is to generate all combinations of some items.
    - Ex: The following program generates all two letter .com Internet domain names.
        - Recall that ord() converts a 1-character string into an integer, and chr() converts an integer into a character.
            - Thus, chr(ord('a') + 1) results in 'b'

![5%208%20Nested%20Loops%2081c77865f6d4476495d83d95e334a003/Untitled.png](5%208%20Nested%20Loops%2081c77865f6d4476495d83d95e334a003/Untitled.png)

- nested loop example that graphically depicts an integer's magnitude by using asterisks, creating what is commonly called a histogram::

![5%208%20Nested%20Loops%2081c77865f6d4476495d83d95e334a003/Untitled%201.png](5%208%20Nested%20Loops%2081c77865f6d4476495d83d95e334a003/Untitled%201.png)