- #### Definition 
	- Distributed database of mappings between hostnames and IP addresses
	- Application layer protocol that runs on top of [[UDP]]

- ##### What is stored within DNS?
	- [[Resource records]]
		- Fields are: name, value, type, TTL

- ##### How does a host receive a [[Domain|domain]] through DNS?
	1. Communicates with [[Local DNS server|local DNS server]] to see if it has address cached
	2. If not, local DNS server communicates with [[Root DNS server|root DNS server]] to retrieve server which is responsible for specific [[Top level domain|top level domain]] host needs
	3. Specific [[Top level domain server|top level domain server]] reaches out to [[Authoritative DNS server|authoritative DNS server]] for domain name
	4. Authoritative DNS server reaches back out to local DNS server with domain name
	5. Finally, local DNS server communicates IP address back to host
