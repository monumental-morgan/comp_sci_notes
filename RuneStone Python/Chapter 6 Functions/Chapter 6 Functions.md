# Chapter 6 Functions

[6.1 Functions](Chapter%206%20Functions%208a16c36206fb478a9c12dfff1b32df49/6%201%20Functions%200e463c91b8184de6aa396936b1bf96df.md)

[6.2/3 Function Return Values & Unit Testing](Chapter%206%20Functions%208a16c36206fb478a9c12dfff1b32df49/6%202%203%20Function%20Return%20Values%20&%20Unit%20Testing%207c58765f3e304a3ab9c553a31bb98e4c.md)

[6.4/5 Variables and Parameters are Local](Chapter%206%20Functions%208a16c36206fb478a9c12dfff1b32df49/6%204%205%20Variables%20and%20Parameters%20are%20Local%20b391f4ecfda04c74842b068e352d6b59.md)

[6.8 Using a main Function](Chapter%206%20Functions%208a16c36206fb478a9c12dfff1b32df49/6%208%20Using%20a%20main%20Function%2074b4ce61f0ea40af83f56bc154190986.md)

[6.9 Program Development](Chapter%206%20Functions%208a16c36206fb478a9c12dfff1b32df49/6%209%20Program%20Development%20a2c12f69732c4ba59890a9b115a25611.md)

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