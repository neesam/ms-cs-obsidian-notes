- ### Purpose
	- Makes it possible to run multiple, independent Operating Systems by using a hypervisor

- ### Bare metal problems solved by VMs
	- Applications might need different Operating Systems
	- Applications might have variable workloads
	- Applications might have conflicting dependencies (e.g., App 1 needs python3, App 2 needs python 2)

- ### Challenges
	- Heavyweight
		- CPU, memory, disk in exchange for extra OS and full set of binaries
	- Overhead
		- OS traditionally assume they're directly on hardware 