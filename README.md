# TFDE_KAN

Repository containing ChebyKAN, KAN (B-spline) and FC networks used to solve a test time-fractional PDE (TFDE).

Abstract: Deep learning has emerged as a promising approach for the numerical solution of fractional partial differential equations, offering flexibility in approximating complex solution spaces. Conventional methods, such as feedforward neural networks (FNNs) or multilayer perceptrons, have been applied to such problems but often require numerous parameters and exhibit limited accuracy when handling fractional-order operators. To address these challenges, we adopt a novel deep learning framework, the Kolmogorov–Arnold Network (KAN), which serves as an alternative to traditional FNNs for solving fractional partial differential equations. The design of KAN is inspired by the Kolmogorov–Arnold representation theorem, enabling efficient functional representation through the composition of univariate transformations. The study explores two configurations of KAN, one employing B-splines and the other using Chebyshev polynomials. Preliminary numerical experiments on one-dimensional fractional problems demonstrate that both variants achieve improved accuracy compared to standard FNNs. 
    
		\textcolor{blue}{The proposed framework’s performance is demonstrated using three numerical experiments, along with visual comparisons and summarized tables.}
## Structure
- `src/` : python package with modules
  - `networks.py` : all network definitions (ChebyKAN, KAN, FNN)
  - `model.py` : `Model` class implementing PDE loss, training, prediction
  - `train.py` : runnable scripts (`show_comparison`, `show_combined`) and CLI-like entrypoints
  - `plot_utils.py` : plotting helpers
  - `utils.py` : small helpers (seed, metrics)
- `requirements.txt` : python dependencies
- `.gitignore`

  
Note: In the same way, we can write the corresponding formulation for the remaining examples.
