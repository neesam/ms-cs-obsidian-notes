- #### What is congestion?
	- Congestion in [[TCP]] occurs when the network becomes overloaded, leading to [[Segment header|packet loss]], delays, or lower throughput. It can happen when the sender transmits data faster than the network can handle


- #### How does congestion happen?
	- Different bandwidths
		- When data passes through network segments with varying bandwidth capacities, congestion can occur. A faster sender may overwhelm a slower network segment, leading to packet loss or delays in transmission
	- Forwarding multiple ports to one
		- When multiple ports forward data to a single destination, such as a [[Server|server]], the shared network path can become a bottleneck.
	- Overloading the [[Router|router]]
		- Routers can become overwhelmed when they have to process too many [[Packet|packets]] at once. When the router's buffer becomes full, packets are dropped, which can trigger [[Congestion control|congestion control]] mechanisms in TCP

- #### What happens when congestion occurs?
	- Packets get dropped by the router
		- Packets get [[Retransmission|retransmitted]] if it is detected that they have been dropped
	- Packet delay

