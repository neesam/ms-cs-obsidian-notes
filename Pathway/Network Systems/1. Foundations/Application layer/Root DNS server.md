- #### Definition
	- First point of contact in resolving domain names to [[IP address|IP addresses]]. Responds to DNS queries by directing them to the appropriate [[Top level domain server|Top Level Domain servers]] (e.g., for .com, .org, etc.)

- ##### When does the Root DNS server come into play?
	- When a client needs to resolve a [[Domain|domain]] name, the request first goes to a root DNS server. The root server doesn't know the exact IP address of the requested domain but points the client to the correct TLD server, which can further direct the query to the authoritative DNS server for that domain

- ##### How many logical root DNS servers are there?
	- 13, named A to M

- ##### How and why do logical root DNS servers exist?
	- Each logical root server is actually backed by many physical servers distributed worldwide to ensure reliability and reduce latency