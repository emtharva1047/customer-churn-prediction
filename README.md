# Customer Churn Prediction

An end-to-end machine-learning project exploring which telecom customers may be at risk of leaving. It includes data-preparation scripts, feature selection, model comparison, a Streamlit dashboard, and project documentation.

## Highlights

- Designed around the IBM Telco Customer Churn benchmark (7,043 rows and 21 columns).
- Compares multiple classification approaches. The project’s model-comparison report records test ROC-AUC values of **0.8471** for tuned Gradient Boosting and **0.8391** for Logistic Regression. These are benchmark results, not production guarantees.
- Per-customer prediction exports and trained model binaries are not included in this source-only repository.

## Run locally

1. Create a Python environment and install dependencies:

   ```bash
   python -m venv .venv
   pip install -r requirements.txt
   ```

2. Obtain the dataset under its source terms and place `Telco-Customer-Churn.csv` in `data/raw/`. See [`DATASET_GUIDE.md`](DATASET_GUIDE.md).
3. Run the numbered scripts in `scripts/` to prepare data and train the model.
4. Launch the dashboard after the pipeline creates its local files:

   ```bash
   streamlit run dashboard/app.py
   ```

Generated data, models, and customer-level prediction exports should remain local; `.gitignore` excludes them.

## Dataset and use

The project guide identifies the benchmark as CC0 / public domain and links to [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn). The dataset is not bundled here. Review its source page and the included guide before reuse.

## Disclaimer

This is a learning and portfolio project. Model outputs should not be used to make real customer decisions without appropriate validation, fairness review, and operational safeguards.

## Archive note

This repository includes the curated source-only bundle `customer-churn-prediction.zip` and the original uploaded archive `Customer churn prediction_.zip`. The original archive is separate from the curated bundle; review its contents and the source terms before reusing or redistributing it.
