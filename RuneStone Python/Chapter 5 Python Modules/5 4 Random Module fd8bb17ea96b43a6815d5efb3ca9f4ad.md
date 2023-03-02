# 5.4 Random Module

We often want to use **random numbers** in programs. Here are a few typical uses:

- To play a game of chance where the computer needs to throw some dice, pick a number, or flip a coin,
- To shuffle a deck of playing cards randomly,
- To randomly allow a new enemy spaceship to appear and shoot at you,
- To simulate possible rainfall when we make a computerized model for
estimating the environmental impact of building a dam,
- For encrypting your banking session on the Internet.

```python
import random

prob = random.random()
print(prob)

diceThrow = random.randrange(1, 7)       # return an int, one of 1,2,3,4,5,6
print(diceThrow)
```

- The `randrange`function generates an integer between its lower and upper argument, using the same semantics as `range`
    - So the lower bound is included, but the upper bound is excluded.
- The `random.random()`function returns a floating point number in the range [0.0, 1.0)
    - The square bracket means “closed interval on the left” and the round parenthesis means “open interval on the right”
        - 0.0 is possible, but all returned numbers will be strictly less than 1.0.

### Example

- In the case shown here, we’ve converted the result of the method call to a number in the range [0.0, 5.0).
- Once more, these are uniformly distributed numbers (all numbers have equal chance

```python
import random

prob = random.random()
result = prob * 5
print(result)
```

### Notes

- Random number generators are based on a **deterministic** algorithm — repeatable and predictable.
- Each time you ask for another random number, you’ll get one based on the current seed attribute, and the state of the seed (which is one of the attributes of the generator) will be updated.