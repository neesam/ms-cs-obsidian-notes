- #### Definition
	- An open-source [[RPC]] (Remote Procedure Call) framework that allows communication between client and server applications in a [[Distributed system|distributed system]], enabling them to call functions on each other as if they were local. It is designed to make inter-service communication faster and more efficient by using **[[Protobut|Protocol Buffers]] (Protobuf)** for data serialization and **HTTP/2** for transport.

- #### Purpose
	- Used to build efficient, scalable, and language-agnostic APIs that facilitate communication between distributed services or microservices in a highly performant manner. It is particularly useful for real-time data streaming, low-latency communication, and when multiple services or clients are built in different programming languages.

- ##### Features of gRPC
	- ###### Protobufs
		- gRPC uses Protocol Buffers (Protobufs), which are a binary serialization format for compact, efficient data encoding
		- Protobufs help define the structure of messages exchanged between client and server and are language-agnostic
	- ###### HTTP/2-based Transport
		- gRPC leverages **HTTP/2**, which provides multiplexing (multiple requests over one connection), header compression, and bidirectional streaming, allowing for better performance and lower latency than traditional HTTP/1.1
	- ###### Language support
		- gRPC is compatible with many programming languages (Go, Python, Java, C++, etc.), making it ideal for cross-language communication

- #### How to use?
	1. Create a .proto file
		-  The `.proto` file defines the structure of the data (messages) and the services (RPC methods) that the client can call
	2. Compile the `.proto` file
		- Use the `protoc` compiler to generate client and server code from the `.proto` file
		- This generates **stubs**, which handle serializing and deserializing data
	3. Create server program
		- Implement the server logic by defining the functions specified in the `.proto` file
	4. Create client
		- Use the generated client stub to make [[RPC]] calls to the serve 