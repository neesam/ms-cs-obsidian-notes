- ### Definition
	- A process that runs in its own namespace (own file directory structure, own network resources, own file descriptors, etc)

- ### Purpose
	- To package apps and their dependencies in isolated, lightweight environments, ensuring consistency across development, testing, and production

- ### What key mechanisms support containerization within the data plane?
	- [[Linux namespace]]
		- What resources and naming of those resources a process sees (file descriptors, IP addresses)
	- cgroup (Control group)
		- Groups processes and allocates resources (CPU, memory) that the kernel enforces