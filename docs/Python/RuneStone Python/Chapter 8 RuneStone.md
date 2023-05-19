# Chapter 8: For & While Loops Revisited

- Recall that the `for`loop processes each item in a list
    - Each item in turn is (re-)assigned to the loop variable, and the body of the loop is executed
    
    ```python
    for f in ["Joe", "Amy", "Brad", "Angelina", "Zuki", "Thandi", "Paris"]:
        print("Hi", f, "Please come to my party on Saturday")
    ```
    
- We have also seen iteration paired with the update idea to form the accumulator pattern
    - we could create a for loop using the `range`to produce the numbers 1 through n.
    - we can start with a running total variable initialized to 0 and on each iteration, add the current value of the loop variable.
    
    Example
    
    ```python
    def sumTo(aBound):
        theSum = 0
        for aNumber in range(1, aBound + 1):
            theSum = theSum + aNumber
    
        return theSum
    
    print(sumTo(4))
    
    print(sumTo(1000))
    ```
    
    # Zach’s Notes
    
    ### Very clever double loop
    
    - Run through two lists in one loop
    
    ```python
    names = ["Aman", "Hritika", "Akanksha"]
    age = [22, 21, 24]
    index = 0
    for i in names:
        print("My Name is ", names[index], "I am ", age[index], "years old")
        index = index + 1
    
    '''Ouput
    My Name is  Aman I am  22 years old
    My Name is  Hritika I am  21 years old
    My Name is  Akanksha I am  24 years old
    '''
    ```
    

# 8.3 The `while` Statement

The example above but with a `while` loop (easier to understand imo)

```python
def sumTo(aBound):
    """ Return the sum of 1+2+3 ... n """

    theSum  = 0
    aNumber = 1
    while aNumber <= aBound:
        theSum = theSum + aNumber
        aNumber = aNumber + 1
    return theSum

print(sumTo(4))

print(sumTo(1000))
```

More formally, here is the flow of execution for a `while` statement:

1. Evaluate the condition, yielding `False` or `True`.
2. If the condition is `False`, exit the `while` statement and continue
execution at the next statement.
3. If the condition is `True`, execute each of the statements in the body and
then go back to step 1.

### Warning

- After the initial test, any following tests come only after the execution of the *whole* body, even if the condition becomes false in the middle of the loop body.
- The body of the loop should change the value of one or more variables so that eventually the condition becomes `False`and the loop terminates.