- ##### Definition
	- An endpoint for sending and receiving data between two machines over a network
	- Serves as an interface between an application and the network stack, allowing communication using protocols such as [[TCP]] or [[UDP]]

- ##### What are the key components of a socket?
	- ###### [[IP address]]
		- Identifies the host machine
	- ###### Port number
		- Identifies the specific process or service on the host

- ##### When does a socket get created?
	- When an application wants to communicate over the network, it creates a socket, binds it to a port, and connects it to another socket on a remote machine, enabling data exchange

- ##### What are the key socket types?
	- ###### TCP socket
		- Provides reliable, connected-oriented communication. The data is transmitted as a continuous stream, and TCP ensures that it arrives correctly and in order
	- ###### UDP socket
		- Provides connectionless communication. The data is sent as independent packets, and there's no guarantee of delivery or order, but it's faster and more efficient for certain applications