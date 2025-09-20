# Black-Litterman with Multiple Benchmark Tracking Error

This repository demonstrates portfolio optimization using the Black-Litterman model, with a focus on tracking error analysis against multiple benchmarks. The project includes both a Python script and a Jupyter notebook for interactive exploration and visualization.

## Features
- Downloads historical price data for selected US tech stocks using `yfinance`.
- Computes log returns, annualized mean returns, and covariance matrix.
- Defines multiple benchmarks: market-cap weighted, equal-weighted, and a tilted benchmark.
- Implements the Black-Litterman model with a sample view (e.g., AAPL expected to outperform MSFT).
- Constructs efficient frontiers for both prior (implied) and Black-Litterman posterior returns.
- Calculates tracking error of portfolios versus each benchmark.
- Visualizes:
  - Efficient frontiers with benchmarks
  - Tracking error vs. target return for each benchmark
  - Optimized portfolios (mean-variance, max Sharpe, higher moments)
- Provides summary statistics and weights for selected portfolios.
- All code is available as a Jupyter notebook for easy experimentation.

## Files
- `black_litterman.py`: Original Python script for the full workflow.
- `black_litterman.ipynb`: Jupyter notebook version with step-by-step code, plots, and explanations.
- `.gitignore`: Ensures `.venv` (Python virtual environment) is not tracked by git.

## How to Use
1. Clone the repository:
   ```sh
   git clone https://github.com/aryangoelcode/Black-litterman-with-multiple-benchmarking-tracking-error.git
   cd Black-litterman-with-multiple-benchmarking-tracking-error
   ```
2. Set up a Python virtual environment and install dependencies:
   ```sh
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   # Or manually install: yfinance numpy pandas matplotlib scipy
   ```
3. Run the Jupyter notebook:
   ```sh
   jupyter notebook black_litterman.ipynb
   ```
   Or run the script directly:
   ```sh
   python black_litterman.py
   ```

## What Has Been Done
- Converted the main Black-Litterman workflow from a Python script to a Jupyter notebook for interactive analysis.
- Added code to download and process real historical data for six major US tech stocks.
- Defined and visualized multiple benchmarks for tracking error analysis.
- Implemented the Black-Litterman model with a sample view and computed posterior returns.
- Built and plotted efficient frontiers for both prior and posterior returns.
- Calculated and visualized tracking error versus target return for each benchmark.
- Added optimizers for mean-variance, max Sharpe ratio, and higher moments, and compared their results.
- Committed all changes to the repository and ensured the `.venv` directory is ignored by git.

## Next Steps
- Experiment with different views in the Black-Litterman model.
- Add more benchmarks or assets.
- Extend the notebook with additional risk/return analytics or constraints.

---

For questions or contributions, please open an issue or pull request.
