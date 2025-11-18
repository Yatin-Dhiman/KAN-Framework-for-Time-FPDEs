# TFDE_KAN

Repository containing ChebyKAN, KAN (B-spline) and FC networks used to solve a test time-fractional PDE (TFDE).

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
