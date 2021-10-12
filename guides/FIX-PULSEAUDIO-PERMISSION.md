# Fix Permission Denied on Pulseaudio

## Tested on

- Manjaro

## Problem

- Pulseaudio will not start, ``pulseaudio --start`` or ``pulseaudio`` returns varying errors around failing to start (may include ``failed to start main.c``)

## Reason

- This is because the main home directory is not owned by you, the user, but rather is under root permissions only, meaning regular users cannot change or start anything that may interact with hardware - in this case, headphones/sound devices.

## Fix

- Run the command [``sudo chown $USER /home/$USER``](https://www.linuxadictos.com/en/solucion-al-problema-permission-denied-e-pulseaudio-main-c.html#Verificar_permisos) to change the ownership (ch-own) to normal user
- Run ``pulseaudio --start`` or ``pulseaudio``

### Audio should now work as intended

- ~5late