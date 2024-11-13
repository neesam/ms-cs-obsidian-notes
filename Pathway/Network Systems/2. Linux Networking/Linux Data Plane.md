- ### Definition
	- Part of the network that processes network traffic within the kernel, enabling fast and efficient packet handling
		- API for each function/table exposed through Netlink sockets

- ### Purpose
	- To ensure efficient and scalable packet forwarding and switching

- ### Utilities
	- Provide abstractions for users to configure various aspects of the data plane
		- Uses APIs provided by the data plane through Netlink sockets

- ### Architecture
	- Driver
		- Communicates with network cards
	- Receive function
		- Parses packet to determine data type
	- Queueing
	- Transmits to driver