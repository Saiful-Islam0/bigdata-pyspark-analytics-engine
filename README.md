# Big Data Lab — Final Group Project

**Course:** Big Data Lab  
**Project type:** Final Group Project  
**Notebook:** `pyspark-bigdata-analytics-engine.ipynb`

## Project summary
Loading the dataset from the specified path into a PySpark DataFrame, inferring the schema, and then perform basic data inspection and null value check. *   The dataset contains 1-minute interval data for BTC/USD with columns: `Timestamp`, `Open`, `High`, `Low`, `Close`, and `Volume`. *   All columns were inferred as `double` type. *   The dataset contains no null values across any of its columns. *   Summary statistics provide insights into the range and central tendency of the numerical columns. *   The absence of null values indicates a clean dataset for initial analysis.

## Table of contents
- [About](#about)
- [Repository structure](#repository-structure)
- [Requirements](#requirements)
- [Setup and run](#setup-and-run)
- [Notebook overview](#notebook-overview)
- [Datasets](#datasets)
- [Results & deliverables](#results--deliverables)
- [Contributors](#contributors)
- [License](#license)
- [Contact](#contact)

## About
This repository hosts the code, notebooks, and documentation for the Big Data Lab final group project. The project demonstrates end-to-end big data workflows: ingesting data, processing/cleaning, scalable analysis (Spark), model building or aggregations, and visualization of results. The primary work is contained in the Jupyter notebook `BIGDATALABFINALGROUP.ipynb`.

## Repository structure
```
/                - repository root
├─ BIGDATALABFINALGROUP.ipynb   - main notebook with the full project workflow
├─ data/                         - recommended location for input datasets (not included)
├─ notebooks/                     - (optional) supporting notebooks
├─ src/                           - (optional) python modules or scripts
├─ requirements.txt               - Python dependencies
└─ README_BIGDATALLAB.md         - this file
```

## Requirements
The notebook uses the following Python libraries (detected from the notebook or commonly used in big-data notebooks):

matplotlib, networkx, numpy, pandas, pyspark, scipy, seaborn

We recommend creating a virtual environment and installing dependencies before running the notebook. Example:

```bash
python -m venv venv
source venv/bin/activate      # Linux / macOS
venv\Scripts\activate       # Windows
pip install -r requirements.txt
```

If you do not have a `requirements.txt`, you can create one with the libraries above, for example:

```
pyspark
pandas
numpy
matplotlib
seaborn
scikit-learn
```

Adjust the list depending on the notebook imports and whether you run on a local Spark installation or a cluster.

## Setup and run
1. Clone the repository:
```bash
git clone https://github.com/Saiful-Islam0/bigdata-pyspark-analytics-engine.git
cd bigdata-pyspark-analytics-engine
```

2. Place datasets in the `data/` folder. The notebook references dataset files; if you don't have them, update the paths accordingly.

3. Start Jupyter Notebook / Lab:
```bash
jupyter lab
# or
jupyter notebook
```

4. Open `BIGDATALABFINALGROUP.ipynb` and run cells in order. If the notebook uses PySpark, ensure `SPARK_HOME` is set and the PySpark environment is configured (or run with `pyspark` kernel).

## Notebook overview
The notebook contains (high-level):
- Data ingestion and exploratory data analysis (EDA)
- Data cleaning and transformation (using Spark/Pandas)
- Aggregation and scalable computations
- Modeling or statistical analysis (if applicable)
- Visualizations and interpretation of results
- Conclusions and future work

Key headings discovered in the notebook (markdown):
- ## Setup pyspark
- ## Loading and understanding data
- ## Summary:
- ### Data Analysis Key Findings
- ### Insights or Next Steps
- ## Data Cleaning and Transformation
- ## Exploratory Data Analysis (EDA)
- ## Feature Engineering
- ## Insights from Feature Engineering
- ## Post-Feature Engineering - Distribution Analysis
- ### Distribution of Engineered Features
- ### Insights from Distribution Analysis of Engineered Features
- ## Data Partitioning
- ## Regression Task
- ## Classification Task
- ## Model Evaluation
- ### Interpretation of Model Performance
- ## Feature Importance Analysis
- ### Insights from Feature Importance Analysis
- ## Conclusion

## Datasets
https://www.kaggle.com/datasets/mczielinski/bitcoin-historical-data


## Reproducibility tips
- Pin package versions in `requirements.txt`.
- If using Spark locally, document the Spark version and memory settings.
- Provide sample subset datasets for quick testing (small CSVs) in `data/sample/`.

## License
This project is provided under the MIT License. Replace or change the license file as needed.

---


