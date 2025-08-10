# Firewall-Configuration

What is a firewall?
A firewall is a network security device or software that monitors and controls incoming and outgoing network traffic based on predefined security rules.
Its main purpose is to act as a barrier between trusted internal networks and untrusted external networks, such as the internet, to prevent unauthorized access.

Stateful & Stateless firewalls
Stateful firewalls keep track of the state of active connections and make decisions based on the context of the traffic, meaning they understand whether a packet is part of an existing connection or a new request. 
Stateless firewalls, on the other hand, inspect each packet individually without considering the context or connection state, making them faster but less intelligent in filtering.

Inbound & Outbound rules
Inbound rules control the network traffic entering a system from external sources, while outbound rules control the traffic leaving the system to external networks.
These rules can allow or block specific ports, IP addresses, or protocols based on the organization’s security policies.

How does UFW simplify firewall management?
UFW (Uncomplicated Firewall) provides a user-friendly command-line interface to manage firewall rules on Linux systems, especially those using iptables. 
It simplifies common tasks like allowing or denying specific ports or services without needing to write complex iptables rules manually.

Why block port 23 (Telnet)?
Port 23 is used by the Telnet protocol, which sends data, including usernames and passwords, in plain text. This makes it vulnerable to interception and exploitation by attackers. Blocking port 23 prevents the use of Telnet and encourages the use of secure alternatives like SSH (port 22).

What are common firewall mistakes?
Allowing too many unnecessary ports and services.
Failing to update firewall rules after changes in the network.
Not testing firewall rules after implementation.
Misconfiguring rules that block legitimate traffic.
Not logging and monitoring firewall activity.

How does a firewall improve network security?
A firewall helps block unauthorized access, prevent data breaches, and stop malicious traffic from entering or leaving the network.
It enforces security policies, filters harmful data packets, and acts as the first line of defense in a layered security approach.

What is NAT in firewalls?
NAT (Network Address Translation) is a process where a firewall modifies network address information in packet headers. 
It allows multiple devices on a private network to share a single public IP address when accessing the internet.
NAT improves security by hiding internal IP addresses from external networks and helps conserve IPv4 addresses.
