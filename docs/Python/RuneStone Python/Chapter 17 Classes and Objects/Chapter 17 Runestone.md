# Chapter 17: Classes and Objects

- [[17.4 User Defined Classes]]

# 17.1 Object-oriented programming (OOP)

- Main [programming paradigm](http://en.wikipedia.org/wiki/Programming_paradigm) used in the creation of new software.
- Developed as a way to handle the rapidly increasing size and complexity of software systems and to make it easier to modify these large and complex systems over time.
- Up to now, some of the programs we have been writing use a [procedural programming](http://en.wikipedia.org/wiki/Procedural_programming) paradigm
- Procedural programming (what we've used up until now) focuses on writing functions or procedures which operate on data
- Object-oriented programming focuses on the creation of objects which contain both data and functionality together
- Usually, each object definition corresponds to some object or concept in the real world
    - The functions that operate on that object correspond to the ways real-world objects interact.

# 17.2 A Change of Perspective

- We wrote functions and called them using a syntax such as `drawCircle(tess)`
    - This suggests that the function is the active agent.
- In object-oriented programming, the objects are considered the active agents.
    - For example, in our early introduction to turtles, we used an object-oriented style. We said `tess.forward(100)`, which asks the turtle to move itself forward by the given number of steps.
    - An invocation like `tess.circle()` says *“Hey tess! Please use your circle method!”*
- This change in perspective is sometimes considered to be a more “polite” way to write programming instructions
- Often times shifting responsibility from the functions onto the objects makes it possible to write more versatile functions and makes it easier to maintain and reuse code.
- The most important advantage of the object-oriented style is that it fits our mental chunking more accurately

# 17.3 Objects Revisited

- In Python, every value is actually an object.
    - Whether it be a turtle, a list, or even an integer, they are all objects.
- An object has a **state** and a collection of **methods (basically a function within an object/class)** that it can perform.
- The state of an object represents those things that the object knows about itself.
- With turtle objects, each turtle has a state consisting of the turtle’s position, its color, its heading, etc.
- Each turtle also has the ability to go forward, backward, or turn right or left.

# 17.5 Improving our Constructor

- Our constructor so far can only create points at location `(0,0)`
- To create a point at position (7, 6) requires that we provide some additional capability for the user to pass information to the constructor.
- Since constructors are simply specially named functions, we can use parameters (as we’ve seen before) to provide the specific information.

```python
class Point:

	""" Point class for representing and manipulating x,y coordinates. """

	def __init__(self, initX, initY):

    	""" Create a new point at the given coordinates. """

	    self.x = initX

		self.y = initY

p = Point(7, 6)
```

- Now when we create new points, we supply the x and y coordinates as parameters. When the point is created, the values of﻿ `initX` and ﻿`initY` are assigned to the state of the object.