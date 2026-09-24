# Lab 1 - Data Collection and Pre-Processing

This project demonstrates an end-to-end data engineering workflow using a public e-commerce sales dataset.

The notebook follows a 12-step process covering ingestion, Python data structures, cleaning, transformation, feature engineering, aggregation, and serialization.

A custom `Transaction` class is used to organize transaction data and apply reusable cleaning and calculation methods.

A secondary country metadata dataset is merged with the sales data to add country-code information.

The final processed dataset is serialized to both CSV and JSON formats for reuse.

## Quick Start

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
jupyter notebook
```

Open `data_collection_preprocessing.ipynb` and run the notebook from top to bottom.

## Data Sources

- Primary dataset: [1000 Sales Records - ExcelBIAnalytics](https://excelbianalytics.com/downloads-18-sample-csv-files-data-sets-for-testing-sales/)
- Secondary metadata: [Country List - DataHub](https://datahub.io/core/country-list)

## Other GitHub Projects

- [Data Engineering & EDA Workshop](https://github.com/JohnBuni/data-engineering-eda)
- [ML Programming Project 1](https://github.com/JohnBuni/MLProgramming_Project1)