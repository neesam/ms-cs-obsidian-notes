- ### Definition
	- A kernel feature that isolates resources for each container, giving it a private view of certain system aspects, such as process IDs, network interfaces, and file systems

- ### Purpose
	- To provide resource isolation, ensuring that each container operates independently of others, enhancing security and preventing interference between apps

- ### What is a root namespace?
	- The initial namespace created by the kernel during system startup
	- All processes and resources are part of this default namespace unless explicitly assigned to a different one