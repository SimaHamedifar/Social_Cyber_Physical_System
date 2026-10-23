# Social Cyber Physical System

A Socially Aware Peer-to-Peer Energy Trading System with Integrated Home Energy Management System (HEMS).

## Project Setup

Follow the steps below to set up the development environment.

### 1. Create a Virtual Environment

It is recommended to use a virtual environment to manage project dependencies.

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2. Install Dependencies

Install the project in editable mode, which will also install the dependencies defined in `pyproject.toml` and `requirements.txt`.

```bash
pip install -e .
```

### 3. Data Preparation

The project expects raw data files to be located in the `data/raw/` directory at the project root. Ensure you have the following data files placed correctly before running the notebooks:

- `data/raw/15minute_data_austin.csv`
- `data/raw/metadata.csv`

The primary data preprocessing logic is located in the Jupyter notebook `src/Agentic_HEMS/data_preprocessing.ipynb`. Run all cells to process the data. This will analyze participant metadata, perform time-series feature engineering, and prepare household data. 
