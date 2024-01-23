# Loopback

A loopback is a special network interface that allows communication with the same device. In IPv4, the loopback address is `127.0.0.1`, and in IPv6, it's `::1`. Loopback is commonly used for local testing and diagnostics, ensuring network functionality without external communication.

# Loopback Test

A loopback test is a diagnostic procedure to check the functionality of a network interface by sending data to its loopback address. The loopback address for IPv4 is `127.0.0.1`, and for IPv6, it's `::1`. 

**Example using `ping` for IPv4:**
```bash
ping 127.0.0.1
```

**Example using `ping` for IPv6:**
```bash
ping6 ::1
```

This sends test messages to your own machine and is commonly used to verify the proper functioning of the local network stack without involving external networks.