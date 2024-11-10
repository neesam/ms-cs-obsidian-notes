- ### Definition
	- Protocol that allows user space utilities to tell kernel ([[Linux Data Plane|data plane]]) how to process traffic

- ### How is it built?
	- Built using [[Socket|sockets]]
		- Each application is a client and server run in the kernel (both sides are connected to each other using a socket)