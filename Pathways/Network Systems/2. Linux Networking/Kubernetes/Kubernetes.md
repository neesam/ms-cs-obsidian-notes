- ### Definition
	- An open-source system that automates the management, scaling, and deployment of containerized applications

- ### Purpose
	- Designed to help users build, deliver, and scale containerized applications faster

- ### Pod
	- Unit of work in Kubernetes
	- Often a single container, but can be multiple
	- Receives a unique IP address in the Kubernetes cluster

- ### YAML
	- Base fields:
		- apiVersion
		- kind
		- metadata
		- spec

- ### Service
	- An abstraction which defines a logical set of pods and a policy by which to access them

- ### Architecture
	- [[Kubelet|Kubelet]]
	- [[etcd|etcd]]
	- [[API server]]
	- [[Scheduler]]
	- [[Controller manager]]