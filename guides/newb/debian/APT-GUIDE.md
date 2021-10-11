# APT Guide

The APT package tool is a very popular package manager tool. It ships default on Debian and Debian based systems.

There are some basic ``apt`` tools which it is worth learning to make using Linux an easier experience.

## List Upgradable Packages

Before you update your system,  it can be helpful to list the upgradable pacakges. To do this, run:

``apt list --upgradable``

Seeing all currently installed packages can be done with:

``apt list --installed``

## Updating

Updating your system is critical to keep apps, packages and the kernel up to date.

``sudo apt update``

This command does not get update the system. It simply looks for new updates, and downloads update information for all the new packages it has detected.

To actually update all the eligible packages, run:

``sudo apt upgrade``

The size of the update will be reported and you will need to confirm your choice.

## Searching for Packages

Searching for new packages can be helpful for a number of reasons. To search, run:

``apt search PACKAGE-NAME``

Often, you already know the package you want to install. To see more information about the package, run:

``apt show PACKAGE-NAME``

This will output important information such as version, dependencies, size of install, etc.


## Installing Packages

By this time, you have probably already installed packages onto your system. To install a new package simply run:

``sudo apt install PACKAGE-NAME(s)``

and replace PACKAGE-NAME with the name of the package you would like to install. You can install multiple packages at the same time if you choose.

#### Install Specific Version

``sudo apt install PACKAGE-NAME=PACKAGE-VERSION``

## Removing Packages

To remove (or uninstall) a package with ``apt``, run:

``sudo apt remove PACKAGE-NAME(s)``

and replace PACKAGE-NAME with the name of the package you would like to remove. You can remove multiple packages at the same time if you choose.

**<ins>IMPORTANT</ins>**

``apt remove`` only removes the binaries of the package. This means that it leaves behind config files and unneeded dependencies.

To remove (or uninstall) a package *and all related config files*, run:

``sudo apt purge PACKAGE-NAME(s)``

## Cleaning/Clearing

If you are running low on space, or want to remove unneeded package details lying around the machine, you can run the following commands.

#### Removing old dependencies

As packages update, they no longer require some dependencies, or transfer to depending on something else. Often the old unused dependencies will remain on your machine until you manually remove them. To remove all unused dependencies:

``sudo apt autoremove``

#### Clear local repository of package files

When you install a package, ``apt`` auto-generates a local copy of the package files. This is to make it much faster to re-install at a later date, and while the files are usually small, as more packages are installed, the local repository can become cluttered and large in size. To clean remove all package files of unneeded packages, run:

``sudo apt autoclean``

If you want to completely clear out the local repository, run:

``sudo apt clean``


--- 

~ Slate