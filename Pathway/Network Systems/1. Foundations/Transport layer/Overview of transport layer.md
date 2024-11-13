- Communication between processes or applications running on a host
- Transport [[Header|header]] is added to [[Packet|packet]]
		- Includes source and destination ports

- #### What are three core properties of the transport layer?
	1.  Assure that what applications send is what is received ([[Reliable transfer|reliable transfer]])
	2. Multiplexing
		- A way to define which application a [[Packet|packet]] is for
	3. [[Congestion control]]

- #### What are the main transport protocols?
	- UDP and [[TCP]]

- #### What are the hallmarks of a connectionless-oriented protocol?
	- Uses destination [[IP address]] addresses and destination port to [[Routing Data|route data]] 
	- Does not require a connection setup phase (no handshake before sending data)
	- The only information stored is the (IP address, port) to process mapping, which means minimal tracking or management by the system

- #### What are the hallmarks of a connection-oriented protocol?
	- Uses a "4-tuple" to uniquely identify each connection: source IP, destination IP, source port, and destination port
	- Requires an initial setup (e.g., TCP's 3-way handshake) to establish a connection before any data can be sent
	- The host must maintain more information (state) about the connection, such as data sequencing, reliability checks, and [[Acknowledgements|acknowledgements]]

- 