# Notebook guide

Run the notebooks from the repository root in numeric order:

1. `01_longitudinal_data_pipeline.ipynb` builds the 60-month applicant representation.
2. `02_lstm_model_screening.ipynb` trains the LSTM baseline and saves test predictions.
3. `03_tabular_pipeline_and_model_screening.ipynb` builds the 929-feature tabular representation and screens five tabular model families alongside the LSTM.
4. `04_sage_credit_experiment.ipynb` trains the full, score-free, and application-only CatBoost experts; constructs out-of-fold predictions; trains the neural gate; evaluates the four score-availability conditions; and produces the final analyses.

Each publication notebook starts with a portable configuration cell. Set `HOME_CREDIT_DATA_DIR` and `SAGE_CREDIT_ARTIFACT_DIR` before launching Jupyter when the raw data or generated artifacts live outside the repository.

Cached outputs and execution counts are intentionally cleared. The notebooks were structurally and syntactically validated for publication, but they were not re-executed in this repository because the raw Kaggle data and large generated artifacts are not included.
