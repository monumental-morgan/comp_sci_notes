-   3 thing you can do with a file
    -   **r** read - you may view the contents of the file/directory
    -   **w** write - you may change the contents of the file/directory
    -   **x** execute - you may execute or run the file if it is a program or script.
-   3 sets of people who can specify permissions
    -   **owner** - a single person who owns the file. (typically the person who created the file but ownership may be granted to some one else by certain users)
    -   **group** - every file belongs to a single group.
    -   **others** - everyone else who is not in the group or the owner.

```bash
ls -l /home/ryan/linuxtutorialwork/frog.png
	-rwxr----x 1 harry users 2.7K Jan 4 07:32 /home/ryan/linuxtutorialwork/frog.png
```

-   The first character identifies the file type. If it is a dash ( - ) then it is a normal file. If it is a d then it is a directory.
-   The following 3 characters represent the permissions for the owner. A letter represents the presence of a permission and a dash ( - ) represents the absence of a permission. In this example the owner has all permissions (read, write and execute).
-   The following 3 characters represent the permissions for the group. In this example the group has the ability to read but not write or execute. Note that the order of permissions is always read, then write then execute.
-   Finally the last 3 characters represent the permissions for others (or everyone else). In this example they have the execute permission and nothing else.

### Change Permissions

-   `chmod` Stands for change file mode bits - mode bits=permission indicators
-   chmod has permission arguments that are made up of 3 components
    -   Who are we changing the permission for? [ugoa] - user (or owner), group, others, all
    -   Are we granting or revoking the permission - indicated with either a plus ( + ) or minus ( - )
    -   Which permission are we setting? - read ( r ), write ( w ) or execute ( x )