
Evaluate how well samples from different batches are mixed together, by checking the batch composition of neighbors.

How to calculate entropy of mixing?
For each sample, 
Calculate its k nearest neighbors.
Probability of its neighbors from each batch.
Convert probability to entropy
Randomly select multiple samples and return average entropy.

If batches are well mixed, batch probabilities are similar, which will result to a large entropy. 


This approach is used in scVI[https://github.com/YosefLab/scvi-tools] and later also used in our scScope. 
