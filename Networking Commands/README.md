# 🧠 Networking for DevOps Engineers – Command Reference

**1. Ping:** To check the reachability of a host on an Internet Protocol (IP)
network.

Usage Example: ping google.com

**2. Traceroute (or traceroute6):**: To display the route and measure transit delays of packets across an
Internet Protocol network.

Usage Example: traceroute google.com

**3. Netstat:**: To display active network connections, routing tables, interface
statistics, masquerade connections, and multicast memberships.

Usage Example: netstat -a

**4. Nmap:**: To discover hosts and services on a computer network, creating a
"map" of the network.

Usage Example: nmap -p 1-1000 target

**5. Tcpdump:**: To capture and analyze network traffic.

Usage Example: tcpdump -i eth0

**6. Ipconfig (Windows) / ifconfig (Linux):**: To display the configuration of network interfaces.

Usage Example (Linux): ifconfig

**7. Dig (Domain Information Groper):**: To query DNS name servers for information about host addresses,
mail exchanges, name servers, and related information.

Usage Example: dig google.com

**8. Nslookup (Windows) / host (Linux):**: To query DNS servers for domain information.
 
 Usage Example (Linux): host google.com

**9. Wireshark:** : A network protocol analyzer for troubleshooting and analysis of the
interactions between network components.

Usage Example: Capture and analyze packets on a specific network interface.

**10. Iperf:**: To measure the TCP and UDP performance of a network.

Usage Example: iperf -s (server) and iperf -c <server-ip> (client).
These tools are invaluable for diagnosing network issues, understanding network
performance, and ensuring the proper functioning of network connections. They remain essential for both network administrators and DevOps engineers in their day-to-day
tasks.
