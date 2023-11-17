# mac_address_changer

## Overview
This Python script allows you to change the MAC address of a network interface on Linux. You can either input a custom MAC address or generate a random one.

## Usage
```bash
python mac_changer.py <interface> [-r] [-m <mac_address>]
<interface>: The network interface name on Linux.
-r, --random: Whether to generate a random MAC address.
-m, --mac <mac_address>: The new MAC address you want to change to.
Example
Change MAC address randomly:

bash
Copy code
python mac_changer.py wlan0 -r
Change MAC address to a specific value:

bash
Copy code
python mac_changer.py wlan0 -m 00:11:22:33:44:55
Dependencies
Python 3.x
How It Works
The script utilizes the subprocess module to interact with Linux commands for manipulating MAC addresses. It includes functions for generating a random MAC, retrieving the current MAC, and changing the MAC address.

License
This project is licensed under the MIT License.
