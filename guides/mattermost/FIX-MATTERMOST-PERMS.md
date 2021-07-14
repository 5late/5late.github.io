# Fix MatterMost Permissions

## Tested on

- Arch (server)

## Problem 

- MatterMost complaining about not having permission to ``data/`` directory, despite the directory being 755 (or even 777 - heh) permissioned

## Reason

- MatterMost does not know it has permissions to ``data/`` directory

## Fix

- Open the ``/lib/systemd/system/mattermost.service`` file with your favorite text editor
- Add the line ``ReadWritePaths=/usr/share/webapps/mattermost/data`` under ``ReadWritePaths=/etc/webapps/mattermost/config.json``
- Stop, then start the ``mattermost.service`` file with:
    - ``sudo systemctl stop mattermost``
    - ``sudo systemctl start mattermost``

## Mattermost should now write/read to the ``data/`` directory

- ~5late
