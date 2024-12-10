- ### Purpose
	- Enable communication between multiple, heterogeneous networks

- ### Addressing
	- Each interface gets an IP address
		- IPv4 - 32 bits in dotted decimal
			- Example: 192.168.0.1
		- IPv6 - 128 bits in hextets (16 bits) separated by a colon
			- Example: 2001:0db8:0000:0000:0000:ff00:0042:8329

- ### Utilities
	- `ip addr`
		- Add IP addresses to devices
		- Each device must have at least one address to use the protocol
		- It is possible to have several different addresses attached to one device
			- Example: `ip addr add dev eth1 10.0.1.2`
	- `ip route`
		- Forwarding management
	- `ip neigh`
		- ARP table management