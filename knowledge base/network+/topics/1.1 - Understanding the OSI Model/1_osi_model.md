# OSI Model

The OSI (Open Systems Interconnection) reference model is a conceptual framework comprising 7 layers, each representing different protocols governing the flow of information across a network.

![OSI MODEL](https://raw.githubusercontent.com/jcooper94/jcooper94/main/knowledge%20base/network%2B/materials/images/osi_model.png)

### Mnemonics:
- Please Do Not Throw Sausage Pizza Away
- All People Seem To Need Data Processing

## Layer 1 - Physical:
Deals with physical connections, cabling, and does not involve specific protocols. Troubleshooting includes running [loopback tests](network/materials/misc/loopback_test.md), testing/replacing cables, and swapping adapter cards.

## Layer 2 - Data Link:
Referred to as "The Switching Layer," it involves Data Link Control Protocols. MAC (Media Access Control) addresses on Ethernet operate at this layer.

## Layer 3 - Network:
Known as the "routing" layer, where IP addresses reside. Devices making forwarding decisions based on IP addresses are at layer 3. Frames are fragmented to traverse different networks, from Ethernet to WAN.

## Layer 4 - Transport Layer:
Named the "post office" layer, responsible for Transmission Control Protocol (TCP) and User Datagram Protocol (UDP).

## Layer 5 - Sessions Layer:
Manages communication between devices, handling start, stop, and restart functions. Involves control protocols and tunneling protocols.

## Layer 6 - Presentation Layer:
Responsible for character encoding, application encryption, often combined with the application layer.

## Layer 7 - Application Layer:
Visible in the browser, includes protocols like HTTP, FTP, DNS, POP3.

### Real-world to OSI model mapping:

- L1 Physical: Cables, fiber optic cables, the signal itself.
- L2 Data Link: Frames, MAC Addresses, Switches.
- L3 Network: IP encapsulation.
- L4 Transport: TCP encapsulation.
- L5 Session: Links the presentation to the transport.
- L6 Presentation: SSL encryption.
- L7 Application: [https://mail.google.com](https://mail.google.com) (What you see on the screen).