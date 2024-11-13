- #### What is [[Congestion|congestion]] collapse?
	- When nearing capacity, goodput decreases rapidly
	- When buffers get full, and sender keeps overloading it, more and more [[Packet|packets]] get dropped and [[Retransmission|retransmitted]]

- #### How do we avoid congestion collapse?
	- Implementation of a fair and efficient stall of the offered load
		- ###### Fair
			- Each flow receives an equal share of the bandwidth of a link
		- ###### Efficient
			- The full bandwidth of a link is used
		- Idea is to get it right at the the intersection of efficient and fair

