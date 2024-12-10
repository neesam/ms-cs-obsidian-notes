- ### Definition
	- Process of modifying the IP addresses and sometimes port numbers of packets as they pass through a network device, like a router or gateway

- ### Purpose
	1. To allow devices with private IP addresses to communicate with external networks via public IPs
	2. To manage limited public IP resources by mapping multiple private addresses to a single public IP
	3. To provide security by masking internal network structures from external access

- ### Example
	- **Static mapping**
		- Each server has both a private and public IP address. Internally, it uses the private IP, but for external communication, the private IP gets statically translated to a public IP at the gateway. This might be used in legacy systems or to provide external access to a local network (LAN)
	- **Dynamic Mapping (NAT with Port Address Translation)**
		- In this scenario, multiple internal devices share a single public IP. The gateway dynamically assigns TCP port numbers to distinguish between devices. This is common in home networks, where all devices have private IPs but share one public IP for external communication
	- **Port Forwarding**
		- Used when you want to run a public server (e.g., Minecraft) on a private network. External requests to a specific port on the public IP are forwarded to the server’s private IP. The gateway manages the translation and directs traffic to the correct internal device based on port numbers