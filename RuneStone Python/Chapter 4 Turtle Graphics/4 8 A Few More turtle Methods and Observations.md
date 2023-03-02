# 4.8. A Few More turtle Methods and Observations

## Turtle methods can use negative angles or distances.

- `tess.forward(-100)`will move tess backwards
- `tess.left(-30)`turns her to the right
- because there are 360 degrees in a circle, turning 30 to the left will leave you facing in the same direction as turning 330 to the right
    - The on-screen animation will differ, though — you will be able to tell if tess is turning clockwise or counter-clockwise
    - This suggests that we don’t need both a left and a right turn method
- There is also a *backward* method: `alex.backward(100)`

## A turtle’s pen can be picked up or put down

- This allows us to move a turtle to a different place without drawing a line
- The methods are `up` and `down`
    - `penup` and `pendown` do the same thing.
- Every turtle can have its own shape. The ones available “out of the box” are
    - `arrow`
    - `blank`
    - `circle`
    - `classic`
    - `square`
    - `triangle`
    - `turtle`

```python
alex.shape("turtle")
```

## You can speed up or slow down the turtle’s animation speed

- Speed settings can be set between 1 (slowest) to 10 (fastest)
- 0 turns off animation and immediately draws shape

```python
alex.speed(10)
```

```python
import turtle
wn = turtle.Screen()
wn.bgcolor("lightgreen")
tess = turtle.Turtle()
tess.color("blue")
tess.shape("turtle")

print(list(range(5, 60, 2)))
tess.up()                     # this is new
for size in range(5, 60, 2):    # start with size = 5 and grow by 2
    tess.stamp()                # leave an impression on the canvas
    tess.forward(size)          # move tess along
    tess.right(24)              # and turn her

wn.exitonclick()
```