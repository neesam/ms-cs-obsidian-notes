- ### Overview
	- **Continuous -> intervals**
		- e.g., income -> 10k increments

- ### Split or merge
	- Recursive splitting or merging
		- Supervised or unsupervised: class labels

- ### Unsupervised discretization
	- **Binning and histogram analysis**:
		- Equal width, equal frequency
			- e.g., grading: 10, 20, ... of 100; 10%, 20%, ... of class
	- **Clustering analysis**:
		- using clusters to identify similar intervals
	- **Intuitive partitioning**:
		- based on general understanding, you can intuitively identify your intervals

- ### Supervised discretization
	- **Pre-determined class labels**
	- **Entropy-based interval splitting**:
		- lower entropy means "purer" class distribution (more similar classes in intervals)
			- entropy measures how diverse your dataset is
	- **X<sup>2</sup> analysis-based interval merging**:
		- lower X<sup>2</sup> value means class is independent of interval