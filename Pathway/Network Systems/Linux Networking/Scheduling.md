- ### Definition
	- A mechanism that determines how packets are forwarded through network devices

- ### Purpose
	1. Given a queue that is starting to fill up, determine what/when to drop
	2. Given multiple queues, determine which packet to transmit next

- ### Queues
	- **Size**
		- Too big - long delays with congestion
		- Too short - leads to a lot of drops
	- **What to drop?**
		- Tail drop:
			- When queue fills up, just drop from the tail
			- **Problem**
				- TCP uses packet loss as an indication of congestion
					- With tail drop, packet loss would occur when congestion reaches peak
		- RED (Random Early Detection), CoDel, FQ-CoDel
			- Drop packets earlier to signal to TCP earlier
	- **What queue to transmit from? (multiple queues)**
		- Strict priority:
			- If top queue has a packet, send that; else look in next
		- Round robin:
			- Cycle through each queue, transmitting one packet from each
		- Fair queuing:
			- Mimic a bit-per-bit multiplexing by computing theoretical departure date for each packet