# Markov Random Fields for Collaborative Filtering

This notebook provides an implementation in Python 2.7 of the algorithm outlined in the paper 
"[Markov Random Fields for Collaborative Filtering](https://arxiv.org/abs/1910.09645)" 
at the 33rd Conference on Neural Information Processing Systems (NeurIPS 2019), Vancouver, Canada.

For reproducibility, the experiments utilize publicly available [code](https://github.com/dawenl/vae_cf) for pre-processing three popular data-sets and for evaluating the learned model. That code accompanies the paper "[Variational Autoencoders for Collaborative Filtering](https://arxiv.org/abs/1802.05814)" by Dawen Liang et al. at The Web Conference 2018. While the code for the Movielens-20M data-set was made publicly available, the code for pre-processing the other two data-sets can easily be obtained by modifying their code as described in their paper.

The experiments in the paper (where an AWS instance with 64 GB RAM and 16 vCPUs was used) may be re-run by following these three steps:
- Step 1: Pre-processing the data (utilizing the publicly available [code](https://github.com/dawenl/vae_cf))
- Step 2: Learning the MRF (this code implements the new algorithm)
- Step 3: Evaluation (utilizing the publicly available [code](https://github.com/dawenl/vae_cf))