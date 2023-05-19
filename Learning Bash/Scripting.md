[](https://ryanstutorials.net/linuxtutorial/scripting.php)[https://ryanstutorials.net/linuxtutorial/scripting.php](https://ryanstutorials.net/linuxtutorial/scripting.php)

-   1st line: the shebang: `#!` List the interpreter you are using. Good practice in case of using script in other conditions.
-   Naming: While Linux is an extension-less system, put the .sh extension for convenience.
-   Comments: start with `#` It is common practice to include a comment at the top of a script with a brief description of what the script does and also who wrote it and when

```bash
# A simple demonstration script
# Ryan 4/2/2021
```

-   `./` Tells the system that you want to run a specified script
-   Script must have execute permissions to run
    -   A good command to run to ensure your script is set up right is `chmod 755 <script>`

### Variables

-   Container for piece of data
-   When we set a variable, we specify it's name, followed directly by an equals sign ( = ) followed directly by the value. (So, no spaces on either side of the = sign.)
-   When we refer to a variable, we must place a dollar sign ( $ ) before the variable name.

```bash
#!/bin/bash
# A simple demonstration of variables
# Ryan 4/2/2021
 
name='Ryan'
echo Hello $name
./variableexample.sh
Hello Ryan
```

### Command line arguments