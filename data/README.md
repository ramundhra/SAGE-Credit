# Data setup

This project uses the [Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk/data) competition data. The raw files are not redistributed here.

Place the following files in `data/raw/`:

```text
application_train.csv
bureau.csv
bureau_balance.csv
credit_card_balance.csv
installments_payments.csv
POS_CASH_balance.csv
previous_application.csv
```

Alternatively, point the notebooks to another directory:

```bash
export HOME_CREDIT_DATA_DIR=/absolute/path/to/home-credit-default-risk
```

Generated feature tables, model files, predictions, and evaluation artifacts are written to `artifacts/` by default. Override that location with `SAGE_CREDIT_ARTIFACT_DIR`.
