# 4.4 Detecting ranges with branches

### Relational Operators

- A **relational operator** checks how one operand's value relates to another, like being greater than.

![4%204%20Detecting%20ranges%20with%20branches%20ed24274e9b7b49b984fe4c680725b9da/Untitled.png](4%204%20Detecting%20ranges%20with%20branches%20ed24274e9b7b49b984fe4c680725b9da/Untitled.png)

### Detecting ranges with if-else statements

![4%204%20Detecting%20ranges%20with%20branches%20ed24274e9b7b49b984fe4c680725b9da/Untitled%201.png](4%204%20Detecting%20ranges%20with%20branches%20ed24274e9b7b49b984fe4c680725b9da/Untitled%201.png)

### Operator chaining

- a < b < c determines whether b is greater-than a but less-than c.
    - Chaining performs comparisons left to right, evaluating a < b first
        - If the result is True, then b < c is evaluated next
        - If the result of the first comparison a < b is False, then there is no need to continue evaluating the rest of the expression.
        
        **Note that a is not compared to c