# ip

## Tested on:

- Arch Linux
- Debian

## Purpose

- The ip command can show and manipulate network devices and more (``man ip`` for more info)

## Basic Command Usage

**``ip a`` / ``ip addr``**

- Lists the network interfaces and related ip/MAC addresses.

**``ip link``**

- List the network devices, and their states (this information is also available in the ``ip a`` command)

**``ip route``**

- Outputs the routing table entry for the device

**``ip neigh``**

- Outputs neighbor objects sharing the same physical link

## Advanced (?) Command Usage

**``ip addr add {IP} dev {interface}``/ ``ip addr del {IP} dev {interface}``**

- Add/remove ip addresses to an interface

**``ip link set {interface} UP/DOWN``**

- Set an interface up or down

~ Slate
