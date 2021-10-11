# Install a Browser

As a new user to Linux, the first few things you may want to do is get things set up to continue with your daily life. The first of those is to install a browser.

## Browsers

- [FireFox](#FireFox)
- [Chromium](#Chromium)
- [Google Chrome](#Google Chrome)
- [Brave](#Brave)

## FireFox

Most Linux distributions come packaged with FireFox out of the box, but installing it is very simple.


#### Installation

Debian:

``sudo apt install firefox``

Arch:

``sudo pacman -S firefox``

#### Uninstalling

Debian:

``sudo apt remove firefox``

Arch:

``sudo pacman -Rdd firefox``


## Chromium

Chromium is an open-source broswer which is nearly identical in nature to Google Chrome. It is easier than Chrome to install, due to its open-source nature, and provides nearly the same functionality as Google Chrome.

#### Installation

Debian:

``sudo apt install chromium``

Arch:

``sudo pacman -S chromium``

#### Uninstalling

Debian:

``sudo apt remove chromium``

Arch:

``sudo pacman -Rdd chromium``

## Google Chrome

Google Chrome doesn't by default have as easy a set up as FireFox and Chromium, but is still fairly simple to install.

#### Installation

Debian:

``cd /tmp`` (creating a temporary install file)

``wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb`` (download the ``.deb`` file for the latest Chrome)

``sudo dpkg -i google-chrome-stable_current_amd64.deb`` (use ``dpkg`` to install Chrome from the ``.deb`` file you downloaded)

Arch:

[Create an ``installs`` folder]

``cd installs``

Get the link from [here](https://aur.archlinux.org/packages/google-chrome/)

``git clone`` [Put the link here](https://aur.archlinux.org/packages/google-chrome/)

