# Chapter 19: Intro to Inheritance
# 19.1 Pillars of Object-Oriented Programming (OOP)
- Object-oriented programming involves four key ideas: encapsulation, information hiding, inheritance, and polymorphism
- **Encapsulation** is the idea that a class can package some data together with the methods that manipulate the data.
    - This is a powerful capability, and the chief idea that distinguishes OOP from structured programming
- **Information Hiding** promotes quality code by allowing objects to protect their state against direct manipulation by code using the object.
    - Python, like many languages, provides mechanisms to achieve information hiding, but is not covered in Runestone Academy: **LEARN THIS**
- **Inheritance** and **polymorphism** are mechanisms that help to enable code reuse and contract-based programming, and are the subject of this chapter.
# 19.2 Intro to Inheritance
- Recall Point class from chapter 17:
```python
class Point:
    
    def __init__(self, initX, initY):
        self.x = initX
        self.y = initY
    
    def distanceFromOrigin(self):
        return ((self.x ** 2) + (self.y ** 2)) ** 0.5
    
    def __str__(self):
        return "x=" + str(self.x) + ", y=" + str(self.y)
    
p = Point(7, 6)
print(p)
```

    x=7, y=6

- Now we want to create a class that works like `Point`, but also keeps track of a short description for the point.
- Create a `LabeledPoint` class by copying and pasting the definition for `Point`, changing the name to `LabeledPoint`, and modifying the class to suit our purposes.
- Inheritance provides a way to reuse the definition of Point without having to copy and paste.
```python
class LabeledPoint(Point):	#This example defines a class named LabeledPoint that inherits from the Point class.
    pass
```

- Putting the name `Point` in parenthesis tells Python that the new class, `LabeledPoint`, begins with all of the methods defined in its parent, `Point`
- For example, we can instantiate LabeledPoint using the Point constructor, and invoke any Point methds we want to on it:
```python
p = LabeledPoint(7,6)
dist = p.distanceFromOrigin()
```

- Now, let’s refine LabeledPoint so that it holds a label, along with the x and y coordinates:
```python
class LabeledPoint(Point):
    
    def __init__(self, initX, initY, label):
        self.x = initX
        self.y = initY
            elf.label = label
    
    def __str__(self):
        return "x=" + str(self.x) + ", y=" + str(self.y) + " (" + self.label + ")"
    
labeledPt = LabeledPoint(7,6,"Here")
print(labeledPt)
```

    x=7, y=6
    x=7, y=6 (Here)

- We redefined two of the methods that LabeledPoint inherits from Point: `__init__()` and `__str__()` This is called _**overriding**_
- When both the parent class and child class have a method with the same name, the method on an instance of the child class executes code in the child’s class