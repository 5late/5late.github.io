# Fix Broken Postgres Permissions

## Tested on

- Arch

## Problem

- Postgress does not ``initdb`` with error ``permission denied``

## Reason

- The ``postgres`` user does not have permissions to modify the directory ``/var/lib/postgres/data``

## Fix

- Run command ``sudo chown postgres /var/lib/postgres/data``


### The init command should now work

- ~5late