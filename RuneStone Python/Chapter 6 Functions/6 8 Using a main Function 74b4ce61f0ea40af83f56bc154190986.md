# 6.8 Using a main Function

- In many programming languages (e.g. Java and C++), it is not possible to simply have statements sitting alone like this at the bottom of the program.
- They are required to be part of a special function that is automatically invoked by the operating system when the program is executed.
- This special function is called **main**

Before:

```python
import turtle

def drawSquare(t, sz):
    """Make turtle t draw a square of with side sz."""

    for i in range(4):
        t.forward(sz)
        t.left(90)

wn = turtle.Screen()          # Set up the window and its attributes
wn.bgcolor("lightgreen")

alex = turtle.Turtle()        # create alex
drawSquare(alex, 50)          # Call the function to draw the square

wn.exitonclick()
```

After:

```python
import turtle

def drawSquare(t, sz):
    """Make turtle t draw a square of with side sz."""

    for i in range(4):
        t.forward(sz)
        t.left(90)

def main():                      # Define the main function
    wn = turtle.Screen()         # Set up the window and its attributes
    wn.bgcolor("lightgreen")

    alex = turtle.Turtle()       # create alex
    drawSquare(alex, 50)         # Call the function to draw the square

    wn.exitonclick()

main()                           # Invoke the main function
```

**Note**

- In Python there is nothing special about the name `main`.  We could have called this function anything we wanted.  We chose `main` just to be consistent with some of the other languages.