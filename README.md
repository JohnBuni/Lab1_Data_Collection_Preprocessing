# Lab 1 - Data Collection and Pre-Processing

This project demonstrates an end-to-end data collection and pre-processing workflow using Python and Jupyter Notebook with a public e-commerce sales dataset.

The notebook follows a 12-step process covering data ingestion, Python data structures, data cleaning, transformation, feature engineering, aggregation, and serialization.

A custom `Transaction` class is used to organize transaction data and provide reusable methods for cleaning and calculations.

A secondary country metadata dataset is merged with the sales data to add country-code information.

The final processed dataset is serialized to both CSV and JSON formats for reuse.

## Project Structure

```text
Lab1_Data_Collection_Preprocessing/
│
├── notebooks/
│   └── .gitkeep
│
├── prompts/
│   └── .gitkeep
│
├── src/
│   └── .gitkeep
│
├── data_collection_preprocessing.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

The `notebooks`, `prompts`, and `src` directories are included as part of the project structure and are currently empty.

## Requirements

Before running the project, make sure you have:

- Python 3 installed
- Git installed
- Visual Studio Code
- Jupyter support in VS Code

## Setup and Installation

### 1. Clone the Repository

Open PowerShell or the VS Code terminal and run:

```powershell
git clone https://github.com/JohnBuni/Lab1_Data_Collection_Preprocessing.git
```

Move into the repository:

```powershell
cd Lab1_Data_Collection_Preprocessing
```

### 2. Open the Project in VS Code

From the repository folder, run:

```powershell
code .
```

Alternatively, open Visual Studio Code, select **File → Open Folder**, and select the `Lab1_Data_Collection_Preprocessing` folder.

### 3. Create a Virtual Environment

In the VS Code terminal, run:

```powershell
python -m venv .venv
```

### 4. Activate the Virtual Environment

On Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

After activation, `(.venv)` should appear at the beginning of the terminal prompt.

### 5. Install the Required Packages

Run:

```powershell
python -m pip install -r requirements.txt
```

This installs the Python libraries required by the project.

### 6. Open the Jupyter Notebook

Open:

```text
data_collection_preprocessing.ipynb
```

in Visual Studio Code.

When prompted to select a Jupyter kernel, select the Python interpreter from the project's `.venv` environment.

You can verify that the notebook is using the correct Python environment by running:

```python
import sys
print(sys.executable)
```

The displayed path should point to the project's virtual environment:

```text
Lab1_Data_Collection_Preprocessing\.venv\Scripts\python.exe
```

### 7. Run the Project

In VS Code, select:

**Restart Kernel → Run All**

Run the notebook from top to bottom so that data collection, cleaning, transformation, analysis, and serialization occur in the intended order.

## Data Sources

The project uses two public data sources:

- **Primary dataset:** [1000 Sales Records - ExcelBIAnalytics](https://excelbianalytics.com/downloads-18-sample-csv-files-data-sets-for-testing-sales/)
- **Country metadata:** [Country List - DataHub](https://datahub.io/core/country-list)

The primary dataset contains sales transaction records used throughout the data collection and pre-processing workflow.

The country metadata dataset provides country-code information that is merged with the sales data during processing.

## Project Output

The workflow produces cleaned and transformed transaction data and demonstrates serialization of the processed dataset into:

- CSV
- JSON

These formats allow the processed data to be stored and reused outside the notebook.

## Other GitHub Projects

- [Data Engineering & EDA Workshop](https://github.com/JohnBuni/data-engineering-eda)
- [ML Programming Project 1](https://github.com/JohnBuni/MLProgramming_Project1)