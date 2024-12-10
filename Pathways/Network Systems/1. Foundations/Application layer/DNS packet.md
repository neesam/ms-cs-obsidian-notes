- ##### What is the message format of a DNS packet?
	- ###### Query and Reply
	- ###### Identification 
		- Reply will match query
	- ###### Flags 
		- Tells if query or reply
	- ###### Questions, answers, authority, additional

- ##### What is the function of the question field in a DNS packet?
	- Specifies the [[Domain|domain name]] being queries and the type of [[Resource records|record]] the client is requesting from the DNS server

- ##### What is the function of the answer field in a DNS packet?
	- Contains the resource records that answer the client's query, including the requested domain's resolved data, such as its IP address

- ##### What is the function of the authority field in a DNS packet?
	- Provides information about the [[Domain Name System (DNS)|DNS]] servers that are [[Authoritative DNS server|authoritative]] for the queried domain
	- Contains resource records pointing to the [[Name server|name servers]] that can provide an authoritative answer for the requested domain

- ##### What is the function of the additional field in a DNS packet?
	- Used to include extra information that may not be directly related to the question being asked but is necessary for processing the DNS response efficiently
	- Typically contains resource records that help with the resolution of the requested query, often providing additional hints to optimize communication
	- Enhances overall efficiency of DNS by reducing the number of requests needed to resolve certain names