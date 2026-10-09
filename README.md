# Churn Prediction

A machine-learning project for preparing customer data, training a churn classifier, and evaluating predictions.

## Project layout

- `data/raw/`: original input files; do not edit these files
- `data/interim/`: temporary cleaned or transformed data
- `data/processed/`: model-ready datasets
- `notebooks/`: exploration and experiments
- `src/churn_prediction/`: reusable project code
- `scripts/`: command-line entry points for repeatable workflows
- `models/`: exported model artifacts and preprocessing pipelines
- `reports/`: metrics, plots, and experiment notes
- `tests/`: automated tests

## Setup

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Workflow

1. Place the source dataset in `data/raw/`.
2. Explore it in `notebooks/`.
3. Put reusable cleaning and feature logic in `src/churn_prediction/`.
4. Run training from `scripts/` and save artifacts under `models/`.
5. Store evaluation output in `reports/`.

The expected target column is not fixed yet; define it in `src/churn_prediction/config.py` when the dataset is available.
