- #### What is the service model TCP provides?
	- Abstraction of a reliable, in order stream

- #### How does TCP allow for [[Reliable transfer|reliable transfer]]?
	- ###### Segment includes a sequence number
		- Indicates which bytes are contained in the segment
		- Receiver can say which bytes in sequence it has received
	- ###### Receiver sends an [[Segment header|acknowledgement]] number to the sender
		- Specifies to the sender what the next byte in the stream it expects to receive
	- ###### Sender performs [[Retransmission|retransmission]]
		- Sender can resend unacknowledged bytes in the stream

- #### What is TCP's "three way handshake"?
	1. Sender will send [[Segment header|sequence number]] to receiver
	2. Receiver will send acknowledgement number and send back another sequence number
	3. Sender will send receiver acknowledgement number
		1. After third step occurs, both sides are ready to send [[Segment header|segments]] to each other

- #### Describe the process of TCP before [[Additive Increase Multiplicative Decrease|AIMD]] starts to take effect
	- It engages in a slow start and increases [[TCP state storing|congestion window]] every acknowledgment instead of every [[Segment header|RTT]]


