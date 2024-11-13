- #### Why do we need reliable transfer?
	1. [[Packet|Frame/Packet]] error
		- Errors may occur at [[Link layer|link layer]]
	2. Drops due to [[Congestion|congestion]]
		- If the incoming rate of items going into packet queue is higher than the outgoing rate, then the packet buffer in the line cards will fill up and dropping of packets will have to occur
	3. Packet reordering
		- Might happen if new, shorter paths get created