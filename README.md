# ARTI303 Assignment 1 — Pandas vs Polars

## Project Overview

This project compares **Pandas** and **Polars** for common data-processing operations using the **Lenskart India** dataset.

The goal is to measure the execution time of both libraries, compare their performance, and observe when Polars provides an advantage over Pandas.

## Dataset

- Dataset: Lenskart India
- Rows: 150,000
- Main columns used:
  - `product_category`
  - `quantity`
  - `unit_price`
  - `discount_percent`
  - `net_sales_amount`
  - `customer_age`

## Libraries

- Python
- Pandas
- Polars
- NumPy

## Operations Compared

The notebook compares Pandas and Polars on the following operations:

1. Reading the CSV file
2. Filtering rows
3. Creating a new column
4. Grouping and aggregation
5. Sorting and taking the top N
6. Chained operations using Polars Lazy API
7. Joining two tables

For each operation, execution time is measured in milliseconds and the speed ratio is calculated.

## Results

The results show that **Polars is generally faster than Pandas** for most of the tested operations.

The largest performance difference was observed in the chained lazy pipeline, where Polars benefited from query optimization and lazy execution.

However, performance can vary depending on the operation, dataset, and computer used for the experiment.

## Project Structure

```text
ARTI303-Group-3--Assignment1/
│
├── Assignment1/
│   ├── ARTI303_Assignment1_PandasVsPolars.ipynb
│   └── Lenskart India.csv
│
├── results/
│   └── benchmark.csv
│
├── requirements.txt
├── .gitignore
└── README.md
How to Run
1. Clone the repository.
2. Create and activate a Python virtual environment.
3. Install the required libraries:
pip install -r requirements.txt
4. Open the Jupyter Notebook:
Assignment1/ARTI303_Assignment1_PandasVsPolars.ipynb
5. Select the project Python environment as the Jupyter kernel.
6. Run the notebook from the beginning using Run All.
Notes
Benchmark results depend on the computer and environment used to run the notebook. Therefore, execution times may differ between team members.
The notebook also records the machine used for the measurements to provide context for the benchmark results.
Team
ARTI303 — Group 3
Assignment 1: Pandas vs Polars
