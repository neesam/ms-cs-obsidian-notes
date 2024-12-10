- ### Definition
	- A virtual local area network is a way to create separate, isolated networks within the same physical network. It works at **Layer 2** of the OSI model (the data link layer) and is used to segment traffic between different groups of devices, even though they are connected to the same physical switches

- ### Tagging
	- VLANs add a special "tag" to network traffic that identifies which VLAN the traffic belongs to 
	- The VLAN tag is added to the Ethernet frame header, allowing switches and other devices to direct traffic based on this tag

- ### Tagged traffic
	- Once the VLAN device (`eth0.2`) is set up, any traffic that passes through it will be tagged with the VLAN ID
	- This tagging happens automatically, and switches or other networking devices can route traffic based on the VLAN ID


- ### Example scenario
	- Imagine a company with two departments: Finance and HR. You could create two VLANs: VLAN 10 for Finance and VLAN 20 for HR. Devices in VLAN 10 (Finance) cannot communicate with devices in VLAN 20 (HR), even though they are on the same switch. This separation increases security and limits network congestion.