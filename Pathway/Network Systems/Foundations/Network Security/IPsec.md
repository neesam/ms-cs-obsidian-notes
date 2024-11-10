- ### How does IPsec function?
	- Creates an encrypted tunnel between two endpoints
		- Can be for whole site or one machine

- ### Where is IPsec commonly used?
	- [[VPN (Virtual Private Network)|VPNs]]

- ### Overview
	- To set up an IPsec tunnel, a protocol (ISAKMP/IKE) is used to set up the parameters and keys used, and authenticate each side
		- The traffic can then be exchanged
	- IPsec uses shared keys for encryption and integrity
		- [[Diffie Hellman]] is a protocol to secretly create and share private keys
	- **Authentication**:
		- Uses following options decided in SA-1 param exchange:
			- Shared private key
			- Digital certificate
		- Authentication step uses keys determined with Diffie Hellman key exchange step
	- **SA-2 Parameter Exchange**:
		- Sets up security association for traffic exchange in case different parameters are desired
		- Used to set up traffic selectors which determine what traffic is allowed through the tunnel (5-tuple of IP src/dest, protocol, transport src/dest)
	- **Traffic Exchange**:
		- Supports several modes:
			- AH (Authenticating Header - provides just integrity) or ESP (Encapsulating Security Payload - provides integrity and confidentiality)
			- Transport (mostly for single endpoint) or tunnel (mostly for whole site)

- #### What problems does IPsec solve?

- #### How would someone eavesdrop through a network?
	- Network provider compelled by government agency or has a rogue employee or a compromised router
	- Misconfiguration in routing directs traffic to the wrong place
	- Route hijacking to intentionally redirect traffic

- #### What software is available for IPsec?