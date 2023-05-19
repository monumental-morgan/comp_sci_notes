# Chapter 6: Functions
- [[6.1 Functions]]
- [[6.2 6.3 Function Return Values & Unit Testing]]
- [[6.4 6.5 Variables and Parameters are Local]]
- [[6.8 Using a main Function]]

# 6.6 Functions calling other Functions

```python
1	def square(x):
2	    y = x * x
3	    return y
4	
5	def sum_of_squares(x, y, z):
6	    a = square(x)
7	    b = square(y)
8	    c = square(z)
9	
10	    return a + b + c
11	
12	a = -5
13	b = 2
14	c = 10
15	result = sum_of_squares(a, b, c)
16	print(result)
```