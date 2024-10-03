- A TCP flow control mechanism that determines the amount of data (in bytes) a receiver can accept without sending an [[Acknowledgements|acknowledgement]]. This prevents [[Congestion|congestion]] and ensures efficient data flow

- #### What is its relationship to congestion control?
	- The receiver window complements [[Congestion control|congestion control]] by limiting the sender's data transmission rate based on the receiver's ability to process incoming [[Packet|packets]]

- #### What is its impact on throughput?
	- A larger window allows for higher throughput since the sender can transmit more data without waiting for acknowledgements, reducing idle time. Conversely, a small receiver window could limit throughput