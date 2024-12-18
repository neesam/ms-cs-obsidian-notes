- ### Rescaling (Min-max normalization)
	- Map attribute values from [min, max] to [min', max']
	- e.g., income range [50k, 200k], map to [0, 1.0]
		![[Pasted image 20241217175815.png]]
	- Allows you to understand what percentile a value falls into in the context of your dataset

- ### Mean normalization
	- e.g., income range [50k, 200k]. mean = 120k
	- v = 100;
	- v' = (100k-120k)/(200k-50k) = -.13

- ### Standardization (z-score normalization)
	- z-score formula