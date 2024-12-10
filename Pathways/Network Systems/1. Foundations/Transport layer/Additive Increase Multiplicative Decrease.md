- ##### Strategy to optimize congested flow rates network wide

- #### Additive Increase
	- Increasing sending rate by 1 max segment size (maximum [[Packet|packet]] size that you can send into the network) every [[Segment header|Round Trip Time]] until loss is detected
- ##### Multiplicative decrease
	- Decrease sending rate by some multiplicative factor (e.g., by half) when loss is detected

- #### Why does AIMD work?
	- All increase for hosts is the same
	- Decrease is proportional to send rate, so converge towards fair line