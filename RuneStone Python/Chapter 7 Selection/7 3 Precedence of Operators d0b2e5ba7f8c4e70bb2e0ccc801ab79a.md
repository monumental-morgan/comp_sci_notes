# 7.3 Precedence of Operators

### Order Of Operations

![7%203%20Precedence%20of%20Operators%20d0b2e5ba7f8c4e70bb2e0ccc801ab79a/Untitled.png](7%203%20Precedence%20of%20Operators%20d0b2e5ba7f8c4e70bb2e0ccc801ab79a/Untitled.png)

# Order Precedence Table

| Level of Precedence | Operator | Description |
| --- | --- | --- |
| 10 (Highest, trumps all) | (expressions...),
[expressions...],
{key: value...},
{expressions...} | Binding or tuple display,
list display,
dictionary display,
set display |
| 9 | x[index], x[index:index],
x(arguments...), x.attribute | Subscription, slicing,
call, attribute reference |
| 8 | ** | Exponentiation
(groups right to left) |
| 7 | -x | Negation |
| 6 | *, /, //, % | Multiplication,
real and integer division,
remainder |
| 5 | +, - | Addition and subtraction |
| 4 | in, not in, is, is not,
<, <=, >, >=, !=, == | Comparisons, including membership
tests and identity tests |
| 3 | not x | Boolean NOT |
| 2 | and | Boolean AND |
| 1 (Lowest, trumps none) | or | Boolean OR |