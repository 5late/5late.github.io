# Check System Resources

Checking your system resources is an important part of being a system administrator. Knowing what processes are using which resources can be helpful to understand how to optimize programs, or which programs can be running 24/7. 

## top

The ``top`` command ships with most distributions of Linux by default, and can be a good way to see which processes are running, and rank them by the resources they are using.

To run ``top``, open a new terminal and simply type the word ``top``, then press enter.

The command line should disappear, and in its place, you should see a list of all the processes running on the system, sorted by the CPU usage.

**View CPU information**

- To view CPU information, while running ``top``, type ``t``. The bar at the top should show CPU usage, and cycle between usage, tasks, and hidden view.

**View Memory information**

- To view memory information, while running ``top``, type ``m``. The bar at the top should show Memory information, and cycle through stats such as how much memory is being used (both in % and in amount/max mem), how much of the swapfile is being used and hidden.

**Colorful!**

- To make the top stats show in color, while running ``top``, type ``z``. The entire top will swap to a more colorful pattern.

- To make the top stats show up in bold, while running ``top``, type ``b``. The stats will be more bolded.

- To edit your colors, while running ``top``, type ``Z``. A menu will pop up where you can select the different parts of the top interface and customize the color they are

**Saving Config**

- If you do not save, once you exit your current session, your changes will be lost. To make your changes permanent, return to the main top interface (close all menus/help menus) and type ``W``, to write your changes to a file stored in your home directory - ``.toprc``.