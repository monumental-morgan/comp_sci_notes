# 7.4 Splitting and joining strings

### split() method

- The string method split() splits a string into a list of tokens.
    - Each **token** is a substring that forms a part of a larger string.
- A **separator** is a character or sequence of characters that indicates where to split the string into tokens.
    - Ex: 'Martin Luther King Jr.'.split() splits the string literal "Martin Luther King Jr." using any whitespace character as the default separator and returns the list of tokens ['Martin', 'Luther', 'King', 'Jr.']
- The separator can be changed by calling split() with a string argument. Ex: 'a#b#c'.split('#') uses the "#" separator to split the string "a#b#c" into the three tokens ['a', 'b', 'c'].

![7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled.png](7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled.png)

![7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled%201.png](7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled%201.png)

### join() method

- The join() string method performs the inverse operation of split() by joining a list of strings together to create a single string
    - Ex: my_str = '@'.join(['billgates', 'microsoft']) assigns my_str with the string 'billgates@microsoft'.
    - The separator '@' provides a join() method that accepts a single list argument

![7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled%202.png](7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled%202.png)

### Using the split() and join() methods together

- The split() and join() methods are commonly used together to replace or remove specific sections of a string.
    - Ex: A programmer may want to change 'C:/Users/Brian/report.txt' to 'C:\\Users\\Brian\\report.txt', perhaps because a different operating system uses different separators to specify file locations

![7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled%203.png](7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled%203.png)

- A programmer may also want to add, remove, or replace specific token(s) from a string.
    - Ex: The program below reads in a URL and checks whether the fourth token (index 3) is 'wiki', as Wikipedia URLs follow the format of [http://language.wikipedia.org/wiki/topic](http://language.wikipedia.org/wiki/topic).
    - If 'wiki' is missing from the URL, the program uses the list method insert() (explained further elsewhere) to correct the URL by adding 'wiki' before index 3.

![7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled%204.png](7%204%20Splitting%20and%20joining%20strings%206b5599426c074effa781683055e5a14f/Untitled%204.png)