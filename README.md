<div align="center">

# ⚡ Big Data Analytics with PySpark

**A progressive series of PySpark labs — from RDD fundamentals to a Formula 1 data analytics mini project.**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logoColor=white)

</div>

---

## 📖 Overview

This repository is a hands-on learning track for **big data processing with Apache Spark (PySpark)**, organized as seven numbered lab folders that build from low-level RDD operations to DataFrame analytics on CSV data. It culminates in a capstone-style **Formula 1 data analysis mini project** covering the full workflow — loading, cleaning, aggregating, correlating, and visualizing decades of F1 race results — complete with a written report and slide deck.

## ✨ Features

- RDD fundamentals: transformations and actions (`map`, `filter`, `reduce`, `collect`)
- Sampling techniques with `sample()` and `takeSample()` on RDDs
- CSV ingestion with schema inspection, column selection, and DataFrame viewing
- Analytical DataFrame operations: `groupBy`/`agg`, filtering, sorting, and derived columns
- F1 mini project: deduplication, null handling, and feature creation (win flag) on a race-results dataset spanning 861 drivers, 211 constructors, and 77 circuits
- Aggregate leaderboards: top drivers/constructors by points, wins, and podium finishes
- Statistical analysis: grid-position vs points correlation, average grid vs finish position per driver
- Seaborn/Matplotlib visualizations (top-driver bars, season trends, finishing-position distributions) plus a PDF report and PPTX deck

## 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Language | Python 3 |
| Big Data Engine | Apache Spark (PySpark — RDD & DataFrame APIs) |
| Data | CSV datasets (students sample data, F1 race results) |
| Visualization | Seaborn, Matplotlib |
| Environment | Jupyter Notebook |

## 📂 Project Structure

```text
BigDataAnalytics/
├── 1.DataTransformation Using PySpark RDD/
│   └── DataTransformation Using PySpark RDD.ipynb   # RDD transformations & actions
├── 2.Collect() Operation with RDD Operations/
│   └── students.csv                                 # Sample dataset for collect() lab
├── 3.Sample() and takeSample() Methods/
│   ├── sample() And takeSample() Methods.ipynb      # RDD sampling techniques
│   └── students.csv
├── 4.Exploring Structure And Contents of CSV File/
│   └── students.csv                                 # CSV structure exploration lab
├── 5.Viewing Data And Selecting Columns/
│   ├── Viewing Data And Selecting Columns.ipynb     # DataFrame viewing & selection
│   └── students.csv
├── 6.Analytical Operations on CSV File/
│   ├── Analytical Operations on CSV File.ipynb      # groupBy, agg, sort, filter
│   └── students.csv
└── 7.F1 Data Analysis Using PySpark(Mini Project)/
    ├── F1_Data_Analytics_Using_PySpark.ipynb        # End-to-end F1 analysis
    ├── f1_analytics_dataset.csv                     # F1 race results dataset
    ├── F1 Data Analytics Report.pdf                 # Written report
    └── F1 Data Analytics.pptx                       # Presentation deck
```

## 🚀 Getting Started

### Prerequisites

- Python 3.9+
- Java 8/11+ (required by Spark)
- Apache Spark 3.x with PySpark
- Jupyter Notebook or JupyterLab

### Installation

```bash
git clone https://github.com/Ankita-Bha/BigDataAnalytics.git
cd BigDataAnalytics
pip install pyspark pandas seaborn matplotlib jupyter
```

### Usage

```bash
jupyter notebook
```

Open any notebook inside the numbered folders and run cells top to bottom — each notebook creates its own `SparkSession`. For the capstone analysis:

```bash
jupyter notebook "7.F1 Data Analysis Using PySpark(Mini Project)/F1_Data_Analytics_Using_PySpark.ipynb"
```

## 📊 Results

The F1 mini project produces (visible in notebook outputs):

- Dataset profile: **861 unique drivers, 211 constructors, 77 circuits** after cleaning
- Leaderboards for career points, race wins, and podium finishes (e.g., Hamilton, Vettel, Alonso among the podium leaders)
- Correlation analysis: points vs starting grid position ≈ **-0.38** (starting further back costs points) and points vs laps completed ≈ **0.25**
- Country-wise race distribution (Italy, USA, and the UK hosting the most recorded entries)
- Season-wise driver point tables for 2023–2024 and a set of summary charts consolidated in the PDF report and slide deck

## 🔮 Future Improvements

- Add the missing notebooks for labs 2 and 4 (currently only their datasets are included)
- Use Spark SQL and window functions for season/era-normalized comparisons
- Package the F1 analysis as a reusable PySpark script with parameterized queries
- Scale up to the full Ergast/Kaggle F1 dataset and benchmark Spark performance
- Add an interactive dashboard (e.g., Streamlit) over the aggregated outputs

## 👤 Author

**Ankita Bhamidimarri** — [@Ankita-Bha](https://github.com/Ankita-Bha)

---

<div align="center">
<sub>⭐ If you found this project useful, consider giving it a star!</sub>
</div>
