IP Address - Unique identifier per device on the network e.g 192.168.1.144

Subnet mask - Used to determine what subnet the device is on e.g 255.255.255.0

If your computer doesn't know what subnet it's on, it doesn't know what information should be sent locally or to the default gateway (Router) to transverse to another network.

Default gateway e.g 192.168.1.1

The router that allows you to communicate outside your local subnet

Loopback Address e.g 127.0.0.1 through 127.255.255.254
You can do a loopback test (ping your loopback address to test TCP/IP stack to troubleshoot local computer connection)

Reserved addresses
Set aside for future use or testing
240.0.0.1 through 254.255.255.254
All "Class E" addresses

Virtual IP Addresses(VIP)
Not associated with a physical network adapter
Virtual machine, internal router address

Automatic Private IP Addressing (APIPA)
Can only communicate to other local devices
No forwarding by routers or the connection is unavailable 
If you see 169.254.0.1 through 169.254.255.254 then that means the DHCP isn't working