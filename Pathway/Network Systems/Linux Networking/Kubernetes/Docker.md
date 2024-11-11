- ### Definition
	- An open-source platform that automates the deployment, scaling, and management of apps using [[Containers|containerization]]

- ### Purpose
	- To ensure consistency across different environments, making apps highly portable and easier to manage

- ### What did Docker bring to containerization?
	- Made it usable with nice packaging

- ### Architecture
	- [[Containers]]
	- [[Images]]
	- Docker daemon
		- Process that runs on each machine you want to run containers on. 
		- Manages the images, starting processes, interfacing to the cgroups, and namespaces
	- Registry
		- Storage for images
		- Enables an interface to pull/push images to/from a local host