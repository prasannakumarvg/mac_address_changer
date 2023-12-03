mac_address_changer project:

# MAC Address Changer

![Screenshot from 2023-12-03 21-34-54](https://github.com/prasannakumarvg/mac_address_changer/assets/123349921/2d11a8f4-7a23-460c-a21f-865779e06c1d)


## Overview
The `mac_address_changer` Python script enables you to change the MAC address of a network interface on Linux. It provides the flexibility to either input a custom MAC address or generate a random one.

## Usage

    python mac_changer.py <interface> [-r] [-m <mac_address>]
    
    <interface>: The network interface name on Linux.
    
    -r, --random: Generate a random MAC address.
    
    -m, --mac <mac_address>: Set the new MAC address.   
    
Example

Change MAC address randomly:

     >  sudo python mac_changer.py wlan0 -r
     
Change MAC address to a specific value:

     >  sudo python mac_changer.py wlan0 -m 00:11:22:33:44:55
     
Dependencies

      Python 3.x

How It Works:

        The script utilizes the subprocess module to interact with Linux commands for manipulating MAC addresses. It includes functions for generating a random MAC, retrieving the current MAC, and changing the MAC address.

License

      This project is licensed under the MIT License.

Contributing:

      Contributions are welcome! Feel free to open issues or submit pull requests. Please follow the contribution guidelines.
