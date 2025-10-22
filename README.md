# Convergence of Clipped SGD on Convex $(L_0,L_1)$-Smooth Functions - Experiment Code

This repository contains Jupyter notebooks that reproduce the experiments from the paper [Convergence of Clipped SGD on Convex $(L_0,L_1)$-Smooth Functions](https://arxiv.org/abs/2502.16492). The experiment setup, results and implementation details are presented in Section 4 and Appendix H.

## Setup
The code was tested on **Google Colab** (Python 3.10). 
- The notebook **RealData.ipynb** uses **GPUs** by default (by using the CuPy library). <br> To use **CPU** instead, simply replace the first import in the notebook with `import numpy as np`. 

## Reproducing the Experiments

Each notebook, when run fully, downloads the generated figures into Google Colab's working directory.

- To run the experiments on the **California Housing Dataset** (figures 1 & 2 in the paper), run **RealData.ipynb** as is. 
- To run the experiments on the **Parkinsons Telemonitoring Dataset** (figures 3 & 4 in the paper): 
  1. Open **RealData.ipynb** and go to the **data setup** subsection.
  2. Comment out the part loading the California Housing Dataset.
  3. Uncomment the part loading the Parkinsons Telemonitoring Dataset. 
  4. Run the full notebook.
- To run the **Synthetic Data** experiments (figures 5 & 6 in the paper), run **SyntheticData.ipynb** as is. 

## Citation
```bibtex
@inproceedings{gaash2025convergence,
  title     = {Convergence of Clipped {SGD} on Convex {(L_0,L_1)}-Smooth Functions},
  author    = { Gaash, Ofir and Levy, Kfir Yehuda and Carmon, Yair},
  booktitle = {Advances in Neural Information Processing Systems (NeurIPS)},
  year      = {2025}
}
