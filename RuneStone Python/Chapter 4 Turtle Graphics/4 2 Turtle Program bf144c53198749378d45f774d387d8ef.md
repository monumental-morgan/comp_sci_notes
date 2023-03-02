# 4.2 Turtle Program

- turtle: python module that creates a data object called a turtle that can be used to draw pictures
- You can tell your turtle to do simple commands such as go forward and turn right.
- As the turtle moves around, if its tail is down touching the ground, it will draw a line (leave a trail behind) as it moves.
- If you tell your turtle to lift up its tail it can still move around but will not leave a trail.
- The program as shown will only draw the first two sides of the rectangle. After line 4 you will have a straight line going from the center of the drawing canvas towards the right. After line 6, you will have a canvas with a turtle and a half drawn rectangle. Press the run button to try it and see.

```python
import turtle # allows us to use the turtles library
wn = turtle.Screen() # creates a graphics window
alex = turtle.Turtle() # create a turtle named alex
alex.forward(150) # tell alex to move forward by 150 units
alex.left(90) # turn by 90 degrees
alex.forward(75) # complete the second side of a rectangle
```

- The turtle module brings the turtle type and screen type.

## Attributes

- Objects can have attributes, similar to editing HTML elements to add color or change size

```python
import turtle
wn = turtle.Screen()
wn.bgcolor("lightgreen") # set the window background color
tess = turtle.Turtle()
tess.color("blue") # make tess blue
tess.pensize(3) # set the width of her pen
tess.forward(50)
tess.left(120)
tess.forward(50)
wn.exitonclick() # wait for a user click on the canvas

```

- When we invoke its `exitonclick` method, the program pauses execution and waits for the user to click the mouse somewhere in the window.
- When this click event occurs, the response is to close the turtle window and exit (stop execution of) the Python program.