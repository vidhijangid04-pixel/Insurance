
# Streamlit Attrition Dashboard & Modeling Toolkit

This package contains a single-file Streamlit application (`app.py`) that provides:
- HR dashboards with 5 actionable charts and filters (job role multi-select + satisfaction slider)
- A Modeling tab to train Decision Tree, Random Forest, and Gradient Boosting models with stratified 5-fold CV and evaluate metrics (confusion matrices, ROC, AUC, precision/recall/f1)
- A Predict tab to upload new datasets and produce predictions (downloadable CSV)

Usage:
1. Upload your CSV file in the sidebar (left). If your dataset has a column named "Attrition" or another binary-like column, select it as the target in the Data tab.
2. Use the Dashboards tab to explore insights and filter by Job Role and Satisfaction columns (choose which columns map to these in the sidebar).
3. Use the Modeling tab to train models and view performance. Use the Predict tab to apply trained models to new data.

Notes:
- The app is deliberately permissive with column names: it auto-detects common target names but also lets you pick the exact target column.
- Missing values are handled using median (numeric) and most-frequent (categorical) imputation during modeling.
- The zipped package contains files at the root (no folders) per your request.

Requirements (no pinned versions):
- streamlit
- pandas
- scikit-learn
- plotly
- matplotlib
- numpy
