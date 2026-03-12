# Pandas Medicine Analysis

## Purpose

This project is a learning exercise where I followed and studied a Kaggle notebook to understand **Pandas** and data analysis. Through this project, I practiced the following techniques:

- **Data loading and inspection** — reading CSVs, examining shape, columns, dtypes
- **Data cleaning** — handling missing values, dropping unnecessary columns, parsing HTML content, string extraction with regex
- **Data transformation** — splitting and exploding columns, computing derived features (unit price), value counts and normalization
- **Descriptive statistics** — summary statistics, duplicate detection, missing value analysis
- **Data visualization** — pie charts, bar charts, histograms, and word clouds using Plotly and Matplotlib

## Dataset

This project uses the [Assorted Medicine Dataset of Bangladesh](https://www.kaggle.com/datasets/ahmedshahriarsakib/assorted-medicine-dataset-of-bangladesh) from Kaggle, which contains data on medicines, generics, manufacturers, dosage forms, drug classes, and indications.

The notebook is based on the Kaggle kernel by [Muhammed Tausif](https://www.kaggle.com/code/muhammedtausif/medicine-analytics-eda), with some "small" modifications to suit my learning preferences and coding style.

## How to Start

### Prerequisites

- Python 3.8+
- A [Kaggle account](https://www.kaggle.com/) with API credentials

### 1. Set up Kaggle API credentials

1. Go to https://www.kaggle.com/settings and click **Create New Token**
2. This downloads a `kaggle.json` file
3. Place it at:
   - **Windows:** `C:\Users\<your-username>\.kaggle\kaggle.json`
   - **Mac/Linux:** `~/.kaggle/kaggle.json`

### 2. Clone the repository

```bash
git clone <repository-url>
cd pandas-medicine-analysis
```

### 3. Create a virtual environment (recommended)

```bash
python -m venv venv
```

Activate it:

- **Windows (Command Prompt):** `venv\Scripts\activate`
- **Windows (PowerShell):** `venv\Scripts\Activate.ps1`
- **Windows (Git Bash):** `source venv/Scripts/activate`
- **Mac/Linux:** `source venv/bin/activate`

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Launch the notebook

```bash
python -m notebook main.ipynb
```

The notebook automatically downloads the dataset from Kaggle into the `data/` folder when you run it, so no manual download step is needed.

## Project Structure

```
pandas-medicine-analysis/
├── README.md
├── requirements.txt
├── main.ipynb      # Main analysis notebook
└── data/                             # Dataset (downloaded via setup)
    ├── medicine.csv
    ├── generic.csv
    ├── manufacturer.csv
    ├── dosage form.csv
    ├── drug class.csv
    └── indication.csv
```
