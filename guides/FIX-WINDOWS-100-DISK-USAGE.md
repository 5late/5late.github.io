# Fix Windows 100% Disk Usage

## [Source](https://www.cleverfiles.com/howto/100-disk-usage-windows-10.html)

## Tested on

- Windows 10 Home

## Problem

- Degraded performance due to the disk being 100% used.

## Reason

- Windows Search has encountered a bug and is using the disk more than it should

## Fix

- Open a CMD prompt as Administrator
    - Right click 'Command Prompt' and click **Run as Administrator**
- Enter ``net.exe stop "Windows search"``

### Disk should now return to normal

#### Note

- While you will still be able to use the Windows Search as usual, Microsoft will complain with this message:

![Microsoft Complaint](./media/microsoft-complain.png)

~ 5late