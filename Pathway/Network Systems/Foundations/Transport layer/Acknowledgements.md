- #### Definition
	- A signal sent from the receiver to the sender to confirm that the data has been received successfully. It is part of TCP's [[Reliable transfer|reliability]] mechanism, ensuring that no data is lost in transmission

- ##### Purpose
	- Provide feedback to the sender, letting it know which [[Segment header|segments]] have been received. This enables the sender to manage [[Retransmission|retransmissions]] if packets are lost or corrupted

- #### Role of duplicate acknowledgements 
	- Indicative of certain packets being missing or out of order. This can trigger TCP's fast retransmit mechanism, which retransmits the missing segment before the timeout occurs