## PDU (Protocol Data Unit)

### Transmission Units
- A different group of data at different OSI layers
### Ethernet operates on a frame of data
- It doesn't care what's inside
### IP operates on a packet of data
- Inside is TCP or UDP, but IP doesn't care
### TCP or UPD
- TCP Segment
- UDP Datagram

# Encapsulation and Decapsulation of Data

![Encapsulattion and Decapsulation](https://raw.githubusercontent.com/jcooper94/jcooper94/main/knowledge%20base/network%2B/materials/images/encapsulation_decapsulation.PNG)

## Ethernet Frame

Each layer has a header and payload

TCP Header :
The header describes or identifies the payload

The TCP header contains important control information called TCP flags

The flags control the payload

-SYN- Synchornize sequence numbers
-PSH- Push data to the application without buffering
-RST- Reset the connection
-FIN- Last packet from the sender

![Encapsulattion and Decapsulation](https://raw.githubusercontent.com/jcooper94/jcooper94/main/knowledge%20base/network%2B/materials/images/ethernet_frame.PNG)

## Maximum Transmission Unit (MTU)
maximum ip packet to transmit (no fragmenting)

fragmentation slows things down
losing a fragment loses and entire packet

Ping with Don't Fragment and force a maximum size of 1472 bytes per ethernet frame.
1500 bytes - 8 byte ICMP header - 20 bytes IP Address = 1472
ping -D -s 1472 8.8.8.8