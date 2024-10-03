- #### When should the sender retransmit a [[Segment header|segment]]?
	- ###### Timeout
		- If the [[Segment header|Estimated Round Trip Time]] is exceeded 
			- Measurement used to determine how long it should take for a segment to go from sender to receiver and an acknowledgement be sent back
	- ###### Duplicate [[Acknowledgements|acknowledgement]]
		- If the receiver sends duplicate acknowledgements (acknowledgements for the same sequence of bytes it is expecting), this is a signal to the sender to retransmit the segment


