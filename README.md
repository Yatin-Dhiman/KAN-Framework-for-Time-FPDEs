# TFDE_KAN

Repository containing ChebyKAN, KAN (B-spline) and FC networks used to solve a test time-fractional PDE (TFDE).

## Structure
- `src/` : python package with modules
  - `networks.py` : all network definitions (ChebyKAN, KAN, Net)
  - `model.py` : `Model` class implementing PDE loss, training, prediction
  - `train.py` : runnable scripts (`show_comparison`, `show_combined`) and CLI-like entrypoints
  - `plot_utils.py` : plotting helpers
  - `utils.py` : small helpers (seed, metrics)
- `requirements.txt` : python dependencies
- `.gitignore`

## How to run
1. Create a virtual environment: `python -m venv .venv && source .venv/bin/activate`
2. Install: `pip install -r requirements.txt`
3. Run examples:
   - `python -m src.train show_comparison`
   - `python -m src.train show_combined`
