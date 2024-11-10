- ### Definition
	- Table used to perform a certain action on an input packet based on rules
		- If packet has certain dstIP or dstPort, drop; else, allow

- ### Default dropping
	- Good practice as default
	- Sets default action to drop and add rules to have an action other than drop