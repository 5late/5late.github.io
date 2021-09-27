# Make a New User: Part 1

So you've got a linux server and successfully ssh'd into the server as ``root``, what now?

Start by making a new user. Making a new user is a good practive, as logging in as root for extended periods of time is not a good security practice.

## Making a New User

``adduser USERNAME``

Swap USERNAME with a name of your choice. 

``usermod -aG sudo USERNAME``

This command adds the user to the ``sudoers`` group.

#### Verify

``su - USERNAME``

``su`` means **S**witch **U**ser. 

``sudo whoami``

This should output ``root``. If it does not, continue below. If it does, log out of the server, and ``ssh`` in again as the new user. (``ssh USERNAME@IP``)

## Troubleshoot

If you arent able to use ``sudo`` as your new user, try editing the ``sudoers`` file.

``EDITOR=nano visudo``

``visudo``

Scroll to the end of the file and add the following line:

``USERNAME ALL=(ALL:ALL) ALL``

Swap USERNAME with your username. Keep the rest of the line as is.

Hit ``CTRL`` + ``O``, then release and hit ``y`` to confirm the save.

Then hit ``CTRL`` + ``X`` to close the file.

[Check.](#verify)

### You should now have sudo privileges

~ Slate