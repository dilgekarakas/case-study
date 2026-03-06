## Exmox Case Study – Marketing, Fraud & EDA

This repository contains my solution for the Exmox Business Analytics / Senior Data Scientist case study.  
The goal is to support two business initiatives:

- **Marketing initiative**: Evaluate the potential impact and design of a loyalty program using customer- and transaction-level data.
- **Fraud initiative**: Propose an automated fraud risk scoring approach to flag high‑risk transactions and support the Fraud team’s review workflow.

### Repository structure

- `src/notebooks/1-exmox-case-eda.ipynb`  
  Exploratory data analysis of the Business Analytics dataset (distributions, segments, basic insights).

- `src/notebooks/2-exmox-case-marketing.ipynb`  
  Customer and segment analysis for the loyalty program, including RFM-style features, a simple CLV estimation, and an XGBoost model to identify high‑value customers.

- `src/notebooks/3-exmox-case-fraud.ipynb`  
  Fraud detection analysis with rule‑based risk scoring, unsupervised anomaly detection (Isolation Forest, LOF), and a proposed risk‑tier workflow for the Fraud team.

- `src/data/Business_Analytics_Dataset_10000_Rows.csv`  
  The input dataset used in all notebooks.

The notebooks are already executed, so results (tables, metrics, plots) are visible directly on GitHub without running any code.

### Environment

Tested with:

- Python 3.12.12
- numpy 2.0.2
- pandas 2.3.3
- matplotlib 3.10.0
- seaborn 0.13.2
- scikit-learn 1.6.1
- xgboost 3.1.3
- lifelines 0.30.3

Install dependencies with:

```bash
pip install -r requirements.txt
```

### How to run the notebooks locally

1. Clone the repository:

```bash
git clone <your-repo-url>.git
cd <your-repo-folder>
```

2. (Optional but recommended) Create and activate a virtual environment.

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Launch Jupyter and open the notebooks:

```bash
jupyter notebook
```

Then open the notebooks from `src/notebooks/` and run all cells from top to bottom.  
The data paths inside the notebooks assume this structure:

- Notebooks in `src/notebooks/`
- Data file in `src/data/Business_Analytics_Dataset_10000_Rows.csv`

