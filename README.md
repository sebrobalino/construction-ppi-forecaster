# construction-ppi-forecaster

Problem/Goal: Forecast PPI for core building materials (e.g., “Lumber”, “Iron & Steel”, “Construction Materials”) using BLS PPI data to anticipate cost movement.

Inputs: Year-Month (YYYY-MM) and Material Type (e.g., Lumber, Iron & Steel, Construction Materials).

Output: Predicted PPI index (1982=100).

Data Source: FRED series WPUSI012011 (Construction Materials), plus WPU081 (Lumber) and WPU101 (Iron & Steel). Monthly, Jan 1947→Aug 2025; CSV download.

Baselines: (1) naïve “next = last observed”, (2) 12-month rolling average.

Metric: MAE (in index points).
