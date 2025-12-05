Replicating the Results
Part 1 — Preprocessing + EDA
Part 2 — Signal + Portfolio (Signal.ipynb)
Files:

price_metrics.parquet — prices of stocks in the universe

sector_map.csv — sector labels of tickers for optimization

factors_std.parquet — features data for clustering

1. Reading the Data

Edit the file path and file reading method accordingly

Read price_metrics.parquet to extract px_last

Load sector maps

2. Baseline 6-1 Momentum

Follow the documentation to generate, plot, and view results for baseline momentum

3. K-Means Feature Selection

Update the file path for factors_std.parquet

Conduct high-level correlation analysis on features (per documentation)

keep_metrics contains the final selection

Resample to month end

4. K Sweep

Sweep K in-sample to determine the best number of clusters

Optional: Save weights to file (depending on environment)

5. Optimization and Trading Cost Implementation

Run in-sample backtest on K = 20 cluster optimized model vs baseline

6. Out-of-Sample Testing

Run out-of-sample backtest (follow documentation)

Part 3 — Robustness + Explanatory Analysis + Exploratory Analysis