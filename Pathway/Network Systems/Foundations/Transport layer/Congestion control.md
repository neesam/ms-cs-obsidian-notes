- #### What resource allocation tactics can be used to deal with [[Congestion|congestion]]?
	- ###### Reservation
		- Reserve bandwidth on each router
	- ###### Feedback and adjust (used by [[TCP]])
		- On hosts, detect  congestion and adjust send rate

- #### How do we know how much to send once congestion has been detected?
	- Host limits sending through a [[TCP state storing|congestion window]]
	- Usage of the following formula:
		- lastByteSent - lastByteAck has to be <= congestion window

- #### What is the strategy to optimize congested flow rates network wide?
	- [[Additive Increase Multiplicative Decrease]]
