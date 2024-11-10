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
	- kubelet
		- Runs on each node
		- Communicates with server in control plane when a pod is created
		- Interacts with Docker to create containers/pods
	- etcd
		- Distributed key value store
		- Stores state for a k8s cluster (info about pods, deployments, etc.)
	- API server
		- Provides a CRUD interface for querying and modifying the cluster state over a REST API
			- Stores state in etcd
	- Scheduler
		- Waits for newly created pods then assigns a node to each new pod
	- Controller manager
		- Runs multiple controllers as processes performing various reconciliation tasks