- ### Purpose
	- Used to set up, maintain, and inspect the tables of IP packet filter rules in the [[Linux Data Plane|Linux kernel]]. Several different tables may be defined

- ### What is in said table?
	- A number of built-in chains and may also contain user-defined chains
	- 4 defined tables
		- filter - default table
		- nat - table which is consulted when a packet that creates a new connection is encountered
		- mangle - used for specialized packet alteration
		- raw - used mainly for configuring exemptions from connection tracking

- ### What is a chain?
	- A set of rules that are evaluated sequentially

- ### What is a rule?
	- [[Match-Action tables|Match-action]] pair
	- Flags:
		- -p, --protocol
		- -s, --source
		- -d, --destination
		- -i, --in-interface
		- -o, --out-interface
		- -m, --match
		- -j, --jump