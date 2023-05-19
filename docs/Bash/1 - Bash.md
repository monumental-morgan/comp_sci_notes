# The Bash Wiki
## Executing Bash in Fish

If fish is your default shell and you want to copy commands from the internet that are written in a different shell language, bash for example, you can proceed in the following way:

Consider, that `bash` is also a command. With `man bash` you can see that there are two ways to do this:

-   `bash` has a switch `c` to read from a string:
    
    `> bash -c SomeBashCommand`
    

or `bash` without a switch, opens a bash shell that you can use and `exit` afterwards.




[[File Manipulation]]

[[Vi Text Editor]]

[[Permissions]]

[[Scripting]]

### Wildcards

-   [](https://ryanstutorials.net/linuxtutorial/wildcards.php)[https://ryanstutorials.net/linuxtutorial/wildcards.php](https://ryanstutorials.net/linuxtutorial/wildcards.php)
-   Allows you to create a pattern defining a set of files or directories.
-   May be used with any command
-   `-` represents zero or more characters
-   **`?`** - represents a single character
-   **`[]`**- represents a range of characters

### Filters

-   Changes how command line accepts text data
-   `head` Prints first lines of text. Default is 10 lines. ex to show only 4 lines:

```bash
head -4 mysampledata.txt
	Fred apples 20
	Susy oranges 5
	Mark watermellons 12
	Robert pears 4
```

-   `tail` Shows last lines of text. Default is 10. ex to show only 3 lines:

```bash
tail -3 mysampledata.txt
	Greg pineapples 3
	Oliver rockmellons 2
	Betty limes 14
```

## Linux Notes

-   Extensions don't matter in Linux, cause the OS looks at the contents not the extension.
    
-   Linux is case sensitive
    
-   Spaces in file names are accepted, but complicate things. Avoid it.
    
    -   Can be avoided by `'quoting'` the spaced name.
-   `.` in front of a filename makes the file hidden. Can still be found with `ls -a`