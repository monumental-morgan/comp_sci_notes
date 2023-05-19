# 7.2 Logical Operators

- There are three **logical operators**: `and`, `or`, and `not`

### `and`

- For example, `x > 0 and x < 10`is true only if `x`is greater than 0 *and* at the same time, x is less than 10

### `or`

- `n % 2 == 0 or n % 3 == 0`is true if *either* of the conditions is true

### `not`

- Finally, the `not`operator negates a boolean expression, so `not  x > y`is true if `x > y`is false

### Truth Tables

- To show how logical operators work

| a | b | a and b | a or b | not a | not b |
| --- | --- | --- | --- | --- | --- |
| T | T | T | T | F | F |
| T | F | F | T | F | T |
| F | T | F | T | T | F |
| F | F | F | F | T | T |

### Python Quick Note:

- CORRECT:
    - `number == 5 or number == 6 or number == 7`
- NOT CORRECT:
    - `number == 5 or 6 or 7`

# 7.2.1 Logical Opposites

| Operator | Definition | Logical Opposites |
| --- | --- | --- |
| == | Equals to | != |
| != | Not Equals to | == |
| < | Less than | >= |
| <= | Less Than or Equal to | > |
| > | Greater Than | <= |
| >= | Greater Than or Equal to | < |
- Understanding these logical opposites allows us to sometimes get rid of `not`operators
- `not`operators are often quite difficult to read in computer code
    - Our intentions will usually be clearer if we can eliminate them.

**Harder to understand:**

```python
if not (age >= 17):
   print("Hey, you're too young to get a driving licence!")
```

**Easier to understand**

```python
if age < 17:
   print("Hey, you're too young to get a driving licence!")
```

### [De Morgan’s Laws](https://en.wikipedia.org/wiki/De_Morgan's_laws)

- Two powerful simplification laws

```python
not (x and y)  ==  (not x) or (not y)
not (x or y)   ==  (not x) and (not y)
```

### Examples

**Harder to Understand**

```python
if not ((phone_charge >= 0.50) and (phone_storage >= .15)):
   print("You cannot restart your phone. Battery too low or not enough free space.")
else:
   print("Updating now...Several restarts may be required.")
```

Easier to Understand

```python
if (phone_charge < 0.50) or (phone_storage < .15):
   print("You cannot restart your phone. Battery too low or not enough free space.")
else:
   print("Updating now...Several restarts may be required.")
```

**Easiest Understanding/Implementation**

```python
if (phone_charge >= 0.50) and (phone_storage >= .15):
   print("Updating now...Several restarts may be required.")
else:
   print("You cannot restart your phone. Battery too low or not enough free space.")
```