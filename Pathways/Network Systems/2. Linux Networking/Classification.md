- ### Definition
	- Inspecting packets to identify what class of traffic they belong to

- ### Purpose
	- To manage and prioritize data flow, improving performance, security, and resource allocation

- ### Mechanisms
	- **Based on packet headers**
		- Classify traffic based on Layer 3/4 headers
			- For example:
				- Classifying traffic destined for port 80 as web traffic
				- Traffic with an IP source of 1.2.3.0/24 pays more for service, so deserves to be in a higher class
	- **Based on Deep Packet Inspection**
		- Classify based on bit patterns or known headers located in the payload
			- Computationally expensive
			- Helps identify traffic that can't be identified at Layers 3 and 4
	- **Fingerprinting**
		- Performance of statistical analysis over many packets can identify traffic
		- Protocols, applications, OSes all have fingerprints, such as distribution of packet sizes, inter-packet gap