# NMap -
Nmap (Network Mapper) is a free, open-source tool for network exploration and security auditing
It is used to discover hosts and services on a computer network by sending packets and analyzing responses.

In this , we have executed various commands for nmap on kali linux OS.

We have executed the following commands -

Nmap 
This command performs a basic network scan of the website sitpune.edu.in, identifying open ports, services, and possibly the IP address of the target host.

Nmap -sC 
Enables Nmap's default script scan, using common NSE (Nmap Scripting Engine) scripts to gather additional information like service versions, vulnerabilities, and more.


nmap --script smb-enum-shares
Runs a script that enumerates SMB (Server Message Block) shares on the target machine, identifying shared folders and network file systems accessible over SMB.


nmap -F
This performs a fast scan, scanning fewer ports (about 100) from Nmap's list of the most commonly used ports, for quicker results.

nmap -sP
Executes a ping scan to discover which hosts are alive on a network. It does not perform port scans, only identifying live hosts.



nmap -PS
Sends SYN packets to the target hosts to detect open ports. This can be useful for hosts that don’t respond to standard ping requests.


nmap -A
Performs an aggressive scan, including OS detection, version detection, script scanning, and traceroute, giving comprehensive information about the target.

nmap -O
Enables operating system detection by analyzing the network stack responses to determine the target host's OS.


nmap -PR
Uses ARP requests to detect live hosts on a local Ethernet network. ARP scans are highly accurate within local networks.

nmap -traceroute
Traces the path packets take to reach the target by displaying each hop along the route from the scanning host to the target host.


nmap -PA
Sends TCP ACK packets to target hosts, checking for response to detect hosts with open ports while bypassing firewalls that block SYN packets.

nmap -PE
Uses ICMP echo requests (traditional "ping" packets) to determine if hosts are online, sending ping requests to elicit replies from the target.

