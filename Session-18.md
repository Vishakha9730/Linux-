# Networking in linux-
# Network-
- Network is system that connrcts two or more computing devices and establish connection between them.
- Networks allow devices to communicate with each other, whether they are in close proximity or across the globe, using various technologies and protocols.

# Protocol- 
- The protocol specifies the rules and format that used for communication.
- Common protocols include TCP (Transmission Control Protocol) and UDP (User Datagram Protocol).
- TCP is connection-oriented and ensures reliable data delivery through mechanisms like acknowledgment and retransmission.
- On the other hand, UDP is connectionless and does not guarantee delivery but is faster and more lightweight.
- The protocol determines how data is formatted, transmitted, and received between devices.

# IP address-
- An IP (Internet Protocol) address is a numerical label assigned to each device connected to a computer network.
- IP addresses are used to identify and locate devices within a network.
- IPv4 addresses are typically written as four decimal numbers separated by dots (e.g., 192.168.1.1), while IPv6 addresses are written in hexadecimal format with colons separating each group (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).

# Port Number-
- A port number is the logical address of each application or process that uses a network or the Internet to communicate.
-  A port number uniquely identifies a network-based application on a computer.
* Examples-
    - SSH: 22
    - HTTP: 80
    - HTTPS: 443
    - MySQL: 3306

# Networking Utilities-

# ifconfig: 
- Used to configure network interfaces, display their configuration.
- It display ip address and mac address of system.

# ip:
- Provides more advanced network configuration options than ifconfig, including routing, addressing.
- ip addr
  - This command displays information about all network interfaces on your system, including their IP addresses, MAC addresses, and other configuration details.
- ip link
  - Displays information about network interfaces (links), such as their state (UP or DOWN), MTU (Maximum Transmission Unit), and Ethernet address (MAC address).

# ping: 
- Test connectivity.
- Verify that a specific host is reachable over the network.
- Diagnose network connectivity issues, such as packet loss or high latency.
- ping <host>

# traceroute / tracepath: 
- Traces the route taken by packets from the source to the destination, showing intermediate hops and round-trip times.
- traceroute [destination]
  
# netstat-
- Displays various network-related information, such as active network connections, routing tables, interface statistics, and more.
### Options:
- -u: instructs netstat to display UDP (User Datagram Protocol) connections. UDP is a connectionless protocol used for sending data in a network.
- -t: netstat to display TCP (Transmission Control Protocol) connections. TCP is a connection-oriented protocol used for reliable communication over a network.
# wget / curl:
- Command-line tools for downloading files from the internet using HTTP, HTTPS, FTP, and other protocols.




