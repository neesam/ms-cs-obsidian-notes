- #### Definition
	- A set of rules and standards that governs how software applications communicate over a network at the highest level of the **OSI model** or **TCP/IP model**.

- ##### What does an application layer protocol define?
	- The format, order, and meaning of the data exchanged between applications, ensuring that the communication is understood by both the sending and receiving ends.

- ##### How do they function?
	- Application layer protocols operate directly on the data that is being transmitted between users or services. They manage specific user-oriented tasks like file transfer, email, web browsing, and remote access.

- ##### What are some examples of application layer protocols?
	- **[[HTTP]] (HyperText Transfer Protocol)**: Used for transferring web pages and resources over the internet.
	- **FTP (File Transfer Protocol)**: Used for transferring files between computers.
	- **SMTP (Simple Mail Transfer Protocol)**: Used for sending email messages.
	- **DNS (Domain Name System)**: Resolves domain names to IP addresses.
	- **SSH (Secure Shell)**: Provides secure remote login and command execution.

- ##### What are some conversion strategies?
	- ###### Canonical Intermediate Form
		- Sender converts its internal representation to some agreed upon format
		- Receiver converts received data into its internal representation
	- ###### Receiver Makes Right
		- Sender transmits data in its internal representation
			- Includes information about representation
		- Receiver converts from the sender's representation to its own representation if needed
				- Works well if assumption is a homogenous infrastructure