# Basic Linux Commands

**``ls``**

- The *list* command. Lists contents of a directory
    - ``ls -l``: list the contents in long listing format

**``cat``**

- Read the contents of a file
    - ``cat -n``: Print number of lines in file, alongside content

**``pwd``**

- **P**rint **W**orking **D**irectory

**``cd``**

- **C**hange **D**irectory
    - Switch to another directory

**``chown``**

- **Ch**ange **Own**ership
    - Change ownership of a file/directory to another user/group

**``chmod``**

- **Ch**ange **Mod**e
    - Change the file mode of a file/directory
    - To read more about file modes, and what they mean, [see this article](https://www.guru99.com/file-permissions.html#4)

**``more``**

- See more of a file, better than ``cat`` for reading large files slowly, rather than spitting the entire file onto the screen.
- Using the ``ENTER`` key will allow you to move down through the file

**``less``**

- Similar to ``more``, but allows you to search through the file with the ``/`` key
- To search, hit ``/`` then type the phrase you would like to search for
    - All accounts of that phrase will be highlighted, starting with the first
- ``q`` to quit, [Don't let this happen!](https://stackoverflow.com/questions/11828270/how-do-i-exit-the-vim-editor)
