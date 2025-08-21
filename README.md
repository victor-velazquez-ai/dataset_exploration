# dataset_exploration

A **professional, end‑to‑end EDA (Exploratory Data Analysis)** template in a single notebook. 
It loads a CSV (or DataFrame), profiles features, handles missing values, detects/removes outliers, 
plots distributions and relationships, computes correlations for numeric and categorical variables, 
and generates a cleaned dataset ready for modeling.

## 📁 Structure
```
dataset_exploration/
├─ README.md
├─ requirements.txt
└─ notebooks/
   └─ 01_general_eda.ipynb
```

## ⚙️ Setup
```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## ▶️ How to use
1. Open `notebooks/01_general_eda.ipynb`.
2. Set `CSV_PATH` (and optional `TARGET_COLUMN`) in the **Load your dataset** cell.
3. Run all cells. The notebook will:
   - Summarize schema, missingness, and cardinality
   - Plot per-feature distributions (numeric & categorical)
   - Detect outliers and (optionally) remove them
   - Compute correlations (Pearson for numeric; Cramér's V for categorical)
   - Analyze target (classification or regression)
   - Save a cleaned CSV to `artifacts/cleaned.csv`