# 3.5 Dictionary Basics

## Creating a dictionary

- A **dictionary** is a Python container used to describe associative relationships.
- A dictionary is represented by the **dict** object type
- A dict object is created using curly braces { } to surround the key:value pairs
    - Ex: players = {'Lionel Messi': 10, 'Cristiano Ronaldo': 7}
- An empty dictionary is created with the expression players = { }
- Why use a dictionary rather than a list?
    - Ex: If a program contains a collection of anonymous student test scores, those scores should be stored in a list. However, if each score is associated with a student name, a dictionary could be used to associate student names to their score.
    - Other examples of associative relationships include last names and addresses, car models and price, or student ID number and university email address.

![3%205%20Dictionary%20Basics%2038998fe3c679418088902878b13f04a6/Untitled.png](3%205%20Dictionary%20Basics%2038998fe3c679418088902878b13f04a6/Untitled.png)

## Accessing dictionary entries

- Dictionaries maintain a left-to-right ordering, dictionary entries cannot be accessed by indexing
- To access an entry, the key is specified in brackets [ ].
    - If no entry with a matching key exists in the dictionary, then a KeyError runtime error occurs and the program is terminated.

![3%205%20Dictionary%20Basics%2038998fe3c679418088902878b13f04a6/Untitled%201.png](3%205%20Dictionary%20Basics%2038998fe3c679418088902878b13f04a6/Untitled%201.png)

## Adding, modifying, and removing dictionary entries

- A new dictionary entry is added by using brackets to specify the key: prices['banana'] = 1.49
- The **del** keyword is used to remove entries from a dictionary: del prices['papaya'] removes the entry whose key is 'papaya'.
    - If the requested key to delete does not exist then a KeyError occurs.

### Adding new entries to a dictionary:

- dict[k] = v: Adds the new key-value pair k-v, if dict[k] does not already exist.
    - Example: students['John'] = 'A+'

### Modifying existing entries in a dictionary:

- dict[k] = v: Updates the existing entry dict[k], if dict[k] already exists.
    - Example: students['Jessica'] = 'A+'

### Removing entries from a dictionary:

- del dict[k]: Deletes the entry dict[k].
    - Example: del students['Rachel']

![3%205%20Dictionary%20Basics%2038998fe3c679418088902878b13f04a6/Untitled%202.png](3%205%20Dictionary%20Basics%2038998fe3c679418088902878b13f04a6/Untitled%202.png)