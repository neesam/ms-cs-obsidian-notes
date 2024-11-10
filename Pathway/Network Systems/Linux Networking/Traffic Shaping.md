- ### Definition
	- Ensuring a given class of traffic conforms to desired properties, such as rates

- ### Purpose
	- For traffic of a given class to conform to some shape

- ### Key properties
	- **Allowed rate**
	- **Burst rate**

- ### Mechanisms
	- **Token bucket - rate limiting**
		- Tokens are added to a bucket at rate ***R***
		- A packet can only be transmitted if there is a token in the bucket
			- Packets have to conform to given rate 
		- Bucket size ***B*** determines burst rate
			- If no traffic for a while, tokens start filling up the bucket
			- Once traffic resumes, there will be enough tokens for all packets, leading to a burst
			- Burst size can be constrained by limiting bucket size