# 4.4/5 for Loops

- idea of repeating same code over again: iteration
- The `for` statement allows is to write programs that implement iteration

```python
for name in ["Joe", "Amy", "Brad", "Angelina", "Zuki", "Thandi", "Paris"]:
    print("Hi", name, "Please come to my party on Saturday!")
		#prints a separate statement with each name in list
```

- **name** in this `for` statement is called the **loop variable**
- Line 2  is the **loop body.** The loop body is always indented. The indentation determines exactly what statements are “in the loop”.  The loop body is performed one time for each name in the list.

# Flow of execution of the for Loop

- **control flow**, or the **flow of execution**
    - interpreter always keeps track of which statement is about to be executed
- Control flow until now has been strictly top to bottom, one statement at a time: sequential
- `for` statement flowchart

![Untitled](4%204%205%20for%20Loops%206605f774e9bd4996816e7dd808a25462/Untitled.png)