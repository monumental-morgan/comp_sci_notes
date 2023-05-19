### Vi Text Editor (command line)

-   Two modes
    -   Insert (input): input or enter content into the file.
    -   Edit: move around the file, delete, copy, etc
-   `vi` ex: `vi firstfile`
    -   If file name does not exist, vi will create one.
-   **`ZZ`** (Note: capitals) - Save and exit
-   **`:q!`** - discard all changes, since the last save, and exit
-   **`:w`** - save file but don't exit
-   **`:wq`** - again, save and exit

### Navigating a file in Vi

-   **`Arrow keys`**- move the cursor around
-   **`j, k, h, l`**- move the cursor down, up, left and right (similar to the arrow keys)
-   **`^ (caret)`** - move cursor to beginning of current line
-   **`$`** - move cursor to end of the current line
-   **`nG`** - move to the **n**th line (eg 5G moves to 5th line)
-   **`G`** - move to the last line
-   **`w`** - move to the beginning of the next word
-   **`nw`**- move forward n word (eg 2w moves two words forwards)
-   **`b`** - move to the beginning of the previous word
-   **`nb`** - move back n word
-   **`{`**- move backward one paragraph
-   **`}`** - move forward one paragraph

> If you type `:set nu` in edit mode within vi it will enable line numbers. I find that turning line numbers on makes working with files a lot easier.

### Deleting Content

-   **x** - delete a single character
-   **nx** - delete n characters (eg 5x deletes five characters)
-   **dd** - delete the current line
-   **dn** - d followed by a movement command. Delete to where the movement command would have taken you. (eg d5w means delete 5 words)

### Undo

-   **u** - Undo the last action (you may keep pressing u to keep undoing)
-   **U (Note: capital)** - Undo all changes to the current line

### Other ways to view files

-   `cat` Main purpose is to join files together, but can be used for just viewing. Harder to use with ;larger files , because the content will fly across the screen and you can only see the last page.
-   less View files with the ability of scrolling up and down
    -   `spacebar` Skip forward a page
    -   `b` Go back a page
    -   `q` Quit