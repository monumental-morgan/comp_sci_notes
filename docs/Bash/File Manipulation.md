-   `PWD` Print Working Directory: Where your terminal is at
    
-   `ls`List of contents in directory
    
    -   `ls -l` Long listing
-   `cd`Change directories
    
-   `man`Brings up manual. ex: `man ls`
    
    -   `man -k search term` Searches every command's manual for search term
    -   `/searchterm` while already in a manual will search within that manual.
        -   `n` Shows next found search term
-   `mkdir` Makes a directory/folder within whatever current directory you are in.
    
    -   `mkdir -p` Makes parent directories (Multiple hierarchy of folders). ex:
        
        ```bash
        mkdir -p linuxtutorialwork/foo/bar
        ```
        
    -   mkdir -v Tell you what it's doing. ex:
        
        ```bash
        mkdir -pv linuxtutorialwork/foo/bar
        mkdir: created directory 'linuxtutorialwork/foo'
        mkdir: created directory 'linuxtutorialwork/foo/bar'
        ```
        
-   `rmdir` Removes/deletes a directory/folder.
    
-   `touch` Will create file if you specify a nonexistent file. Is also used modify access and modification times on a file (though can still be detected with some digging).
    
-   `cp` Can copy a file or directory. `cp -r` copies the directory and any sub-directories. ex:
    

```bash
ls
    barney example1 foo
cp foo foo2
    cp: omitting directory 'foo'
cp -r foo foo2
ls
    barney example1 foo foo2
```

-   `mv` Move file or directory. ex:

```bash
ls
	barney example1 foo foo2
mkdir backups
mv foo2 backups/foo3
mv barney backups/
ls
	backups example1 foo
```

-   **Line 3** We created a new directory called backups.
    
-   **Line 4** We moved the directory foo2 into the directory backups and renamed it as foo3
    
-   **Line 7** We moved the file barney into backups. As we did not provide a destination name, it kept the same name.
    
    ### Renaming files with `mv`
    

```bash
ls
	backups example1 foo
mv foo foo3
ls
	backups example1 foo3
cd ..
mkdir linuxtutorialwork/testdir
mv linuxtutorialwork/testdir /home/ryan/linuxtutorialwork/fred
ls linuxtutorialwork
	backups example1 foo3 fred
```

-   **Line 3** We renamed the file foo to be foo3 (both paths are relative).
-   **Line 6** We moved into our parent directory. This was done only so in the next line we can illustrate that we may run commands on files and directories even if we are not currently in the directory they reside in.
-   **Line 8** We renamed the directory testdir to fred (the source path was a relative path and the destination was an absolute path).

### Removing files or directories

-   `rm`
-   `rm -r` Remove non empty directories
    -   `rm -ri` Adds confirmation prompt