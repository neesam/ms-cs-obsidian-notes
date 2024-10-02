- #### When should the sender retransmit a [[Datagram header|datagram]]?
	- Timeout
		- If the Estimated Round Trip Time is exceeded 
			- Measurement used to determine how long it should take for a datagram to go from sender to receiver and an acknowledgement be sent back
	- Duplicate [[Acknowledgements|acknowledgement]]
		- If the receiver sends duplicate acknowledgements (acknowledgements for the same sequence of bytes it is expecting), this is a signal to the sender to retransmit the datagram


