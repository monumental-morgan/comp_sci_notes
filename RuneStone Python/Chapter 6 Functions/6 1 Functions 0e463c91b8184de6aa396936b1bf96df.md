# 6.1 Functions

- In Python, a **function** is a named sequence of statements that belong together
- Purpose: organize program into chunks

Syntax:

```python
def name( parameters ):
    statements
```

- In a function definition, the keyword in the header is `def`, which is followed by the name of the function and some *parameters* enclosed in parentheses
- the parameter list is more specifically known as the **formal parameters**
- When you use a function, you provide values to the formal parameters.
- Even if a function call needs no arguments, the parentheses `( )`after the function name are *required*. This can lead to a difficult bug:  A function name without the parenthesis is a legal expression *referring* to the function; for example,`print`and `alex.penup`, but they do not *call* the associated functions.

### docstrings

- If the first thing after the function header is a string (some tools insist that it must be a triple quoted string), it is called a **docstring** and gets special treatment in Python and in some of the programming tools.
- Another way to retrieve this information is to use the interactive interpreter, and enter the expression `<function_name>.__doc__`, which will retrieve the docstring for the function.
    - So the string you write as documentation at the start of a function is
    retrievable by python tools *at runtime.*
- By convention, Python programmers use docstrings for the key documentation of their functions.

### Function Call

- Defining a new function does not make the function run. To do that we need a
**function call**. This is also known as a **function invocation**
- Function calls contain the name of the function to be executed followed by a list of values in parentheses, called *arguments*, which are assigned to the parameters in the function definition.

```python
import turtle

# this is the function that will be called
def drawSquare(t, sz):
    """Make turtle t draw a square of with side sz."""

    for i in range(4):
        t.forward(sz)
        t.left(90)

wn = turtle.Screen()          # Set up the window and its attributes
wn.bgcolor("lightgreen")

alex = turtle.Turtle()        # create alex
drawSquare(alex, 50)          # Call the function to draw the square

alex.penup()
alex.goto(100,100)
alex.pendown()

drawSquare(alex,75)           # Call the function again to draw another square

wn.exitonclick()
```