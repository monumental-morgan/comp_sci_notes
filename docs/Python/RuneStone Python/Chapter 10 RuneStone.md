# Chapter 10: Lists

- A list within another list is said to be **nested** and the inner list is often called a **sublist**.

```python
["hello", 2.0, 5, [10, 20]]
```

- `in` and `not in` are boolean operators that test membership in a sequence. We used them previously with strings and they also work here.
- Again, as with strings, the `+` operator concatenates lists. Similarly, the `*` operator repeats the items in a list a given number of times.

```python
a_list = ['a', 'b', 'c', 'd', 'e', 'f']
print(a_list[1:3])
print(a_list[:4])
print(a_list[3:])
print(a_list[:]) 
```

- `b = a[:]   # make a clone using slice`
- List Methods

![[Pasted image 20230519154733.png]]

- It is also important to realize that with append, the original list is simply modified. On the other hand, with concatenation, an entirely new list is created.