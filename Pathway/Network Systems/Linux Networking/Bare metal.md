- ### Definition
	- A physical computer server that is used by a single consumer
	- Provides access to server's processing power, memory, and storage

- ### Architecture
	1. Level 1 - Hardware (NIC, Disk, CPU, Mem)
	2. Level 2 - Operating System (Windows, Linux)
		- Responsible for tasks such as CPU scheduling, memory management, and the network stack
	3. Level 3 - Binaries / Libraries (Ubuntu, Arch, Windows 7)
		- Responsible for files, package management, and commands
	4. Level 4 - Applications

- ### Challenges
	- Resource wastage (using only part of a server), so want to run multiple applications on the same server
	- Applications might need different Operating Systems
	- Applications might have variable workloads
	- Applications might have conflicting dependencies (e.g., App 1 needs python3, App 2 needs python 2)
		- Sometimes complex to resolve