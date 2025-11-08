# construction-ppi-forecaster

## Problem/Goal 
Forecast PPI for core building materials (e.g., “Lumber”, “Iron & Steel”, “Construction Materials”) using BLS PPI data to anticipate cost movement.

## Inputs
Year-Month (YYYY-MM) and Material Type (e.g., Lumber, Iron & Steel, Construction Materials).

## Output
Predicted PPI index (1982=100).

## Data Source
FRED series WPUSI012011 (Construction Materials), plus WPU081 (Lumber) and WPU101 (Iron & Steel). Monthly, Jan 1947→Aug 2025; CSV download.

## Metric
MAE (in index points).

## Baseline Implementation (Milestone)
For this milestone, a **naïve baseline** model has been implemented:  
> The next month’s PPI equals the previous month’s observed PPI.  

The baseline uses the **Construction Materials (WPUSI012011)** dataset only.  
Additional materials (Lumber and Iron & Steel) will be added in later stages.

---

## Input / Output Examples
The figures below show the first few data points from the input and predicted output used in the baseline:

**Input Example:**  
![Input Example](images/input_example.png)

**Output Example:**  
![Output Example](images/output_example.png)

---
