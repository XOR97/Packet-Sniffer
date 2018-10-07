# Packet Sniffer

Packet Sniffer is a program to get access to the data flowing through your router/ethernet. Any kind of data can be sniffed from the
browser.

Needs Super-User permission for certain utilities to function.

## Description
The file `sniffer.py` when run with python 3 will listen to packets recieved from the socket connection. On receiving the ethernet frame, the program
will break it into individual pieces to ascertain the kind of Protocols. i.e `IPv4/IPv6` and `ICMP,TCP,UDP` (`ICMP: Internet Control
Message Protocol`, `TCP: Transmission Control Protocol (Most Common)`, `UDP: User Datagram Protocol`). Each protocol incorporates discrete
byte information. So the method to unpack the data is distinct. In all the cases though, we'll get Source and Destination Ports (MAC Addresses).

Useful for finding out the bottlenecks in your network or just spying on someone :smiling_imp:
