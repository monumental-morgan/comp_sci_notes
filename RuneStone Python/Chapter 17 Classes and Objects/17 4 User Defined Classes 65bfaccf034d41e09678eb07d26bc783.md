# 17.4 User Defined Classes

- We’ve already seen classes like `str` `int` `float` and `turtle`
- In many cases when we are solving problems we need to create data objects that are related to the problem we are trying to solve. We need to create our own classes.

### Walk-through Example

- `point` object
    
    ![https://remnote-user-data.s3.amazonaws.com/JaQvNk6aYMkR7QMpDoebO_X4102A5_6D9sL8_XIoMkeyYukqktPihWx9VYeNjB83isMd5zOvOj-rRFpRChzYJ8pD9d_QMnkG51WKLU7_Q4q79QhEZWdFVyWjqQ6S_Mxm.png](https://remnote-user-data.s3.amazonaws.com/JaQvNk6aYMkR7QMpDoebO_X4102A5_6D9sL8_XIoMkeyYukqktPihWx9VYeNjB83isMd5zOvOj-rRFpRChzYJ8pD9d_QMnkG51WKLU7_Q4q79QhEZWdFVyWjqQ6S_Mxm.png)
    
- Some of the typical operations that one associates with points might be to ask the point for its x coordinate, `getX` , or to ask for its y coordinate, `getY`
    
    ![https://remnote-user-data.s3.amazonaws.com/7o8sGQzwfOjXkK_F7vbgLA9icHspK81Zc8GLkR7Qav-FTr-gJe20yzzWPieN6Xv5ucek2rkAJicP_w5A_9CGS4-Wym01vL4aQyv_Zdxzggz_E2xwN7OIR2TLZCR9ubSQ.png](https://remnote-user-data.s3.amazonaws.com/7o8sGQzwfOjXkK_F7vbgLA9icHspK81Zc8GLkR7Qav-FTr-gJe20yzzWPieN6Xv5ucek2rkAJicP_w5A_9CGS4-Wym01vL4aQyv_Zdxzggz_E2xwN7OIR2TLZCR9ubSQ.png)
    
- Now that we understand what a `point` object might look like, we can define a new **class**.
- We’ll want our points to each have an `x` and a `y` attribute, so our first class definition looks like this:

```python
class Point:
    """ Point class for representing and manipulating x,y coordinates. """

    def __init__(self):
        """ Create a new point at the origin """
        self.x = 0
        self.y = 0
```

- Class definitions can appear anywhere in a program, but they are usually near the beginning (after the `import` statements)
- The syntax rules for a class definition are the same as for other compound statements.
    - Header which begins with the keyword, `class` , followed by the name of the class, and ending with a colon.
- If the first line after the class header is a string, it becomes the docstring of the class, and will be recognized by various tools. **DON'T FORGET DOCSTRINGS**
    - This is also the way docstrings work in functions.
- Every class should have a method with the special name `__init__`
    - This **initializer method**, often referred to as the **constructor**, is automatically called whenever a new instance of our `Point` object is created.
    - It gives the programmer the opportunity to set up the attributes required within the new instance by giving them their initial state values
        - The `self` parameter (you could choose any other name, but nobody ever does!) is automatically set to reference the newly-created object that needs to be initialized.

```python
class Point:
    """ Point class for representing and manipulating x,y coordinates. """

    def __init__(self):
        """ Create a new point at the origin """
        self.x = 0
        self.y = 0

p = Point()         # Instantiate an object of type Point
q = Point()         # and make a second point
```

- During the initialization of the objects, we created two attributes called x and y for each, and gave them both the value 0.
- Two `Points` have been created, each having an x and y coordinate with value 0.
    
    ![https://remnote-user-data.s3.amazonaws.com/vEZNp4_A17ayZE2VCVFvc4_radK-yMwlNgv7UQLp-EvN3Y4uKG1bH6uYfnCdwnZ8YJDQFdMWe2dAnunceRJ0xdRyxrPinNUTXL2nFbfYRiaE1GXgdlmeCDXHF0_NMZK5.png](https://remnote-user-data.s3.amazonaws.com/vEZNp4_A17ayZE2VCVFvc4_radK-yMwlNgv7UQLp-EvN3Y4uKG1bH6uYfnCdwnZ8YJDQFdMWe2dAnunceRJ0xdRyxrPinNUTXL2nFbfYRiaE1GXgdlmeCDXHF0_NMZK5.png)
    
- **Note**
    - The assignments are not to `x` and `y`, but to `self.x` and `self.y`. The attributes `x` and `y` are *always* attached to a particular instance. The instance is always explicitly referenced with dot notation.
- The variables `p` and `q` are assigned references to two new `Point` objects
- A function like `Turtle` or `Point` that creates a new object instance is called a **constructor**
- Every class automatically uses the name of the class as the name of the constructor function.
- The definition of the constructor function is done when you write the `__init__` function.