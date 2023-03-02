# Chapter 5 Python Modules

[5.3 Math Module](Chapter%205%20Python%20Modules%20e0de45ab5f37403d9cb8f3b6b0d26267/5%203%20Math%20Module%20e5b5d897f3cd42b890b2b25d650da8ea.md)

[5.4 Random Module](Chapter%205%20Python%20Modules%20e0de45ab5f37403d9cb8f3b6b0d26267/5%204%20Random%20Module%20fd8bb17ea96b43a6815d5efb3ca9f4ad.md)

[5.5 Creating Modules](Chapter%205%20Python%20Modules%20e0de45ab5f37403d9cb8f3b6b0d26267/5%205%20Creating%20Modules%20406c43185af94d859d7fab02a9e6658b.md)

# 5.1. Modules and Getting Help

- A module is a file containing python definitions and statements intended for use in other python programs
- Many python modules come with python as part of the standard library
- The [Python Documentation](http://docs.python.org/py3k/) site for Python version 3 is an extremely useful reference for all aspects of Python
- The site contains a listing of all the standard modules that are available with Python (see [Global Module Index](http://docs.python.org/py3k/py-modindex.html))
- You will also see that there is a [Language Reference](http://docs.python.org/py3k/reference/index.html) and a [Tutorial](http://docs.python.org/py3k/tutorial/index.html) (mostly aimed at people who are already familiar with another programming language), as well as installation instructions, how-tos, and frequently asked questions

# 5.2 More About Using Modules

- One of the most important things to realize about modules is the fact that they are data objects, just like any other data in Python
- The first thing we need to do when we wish to use a module is perform an `import`
    - the statement `import turtle` creates a new name, `turtle`, and makes it refer to a module object
- In order to use something contained in a module, we use the **dot
 notation**, providing the module name and the specific item joined together with a “dot”.
    - to use the `Turtle`class, we say `turtle.Turtle`