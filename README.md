# NBA Player Stats Analysis with PySpark

This project presents a comprehensive analysis of NBA player statistics using Apache Spark (PySpark). The analysis focuses on advanced basketball metrics across seasons, including trends, player segmentation, and anomaly detection.

## Project Overview

The dataset contains season-by-season statistics of NBA players. The goal of this project is to explore and understand player efficiency, development trends, and statistical relationships using scalable big data tools.

Key metrics include:
- **PER (Player Efficiency Rating)**
- **TS% (True Shooting Percentage)**
- **Win Shares (WS)**
- **Experience and Age**
- **Rebounding and Scoring Rates**

The dataset was analyzed using various PySpark modules including DataFrame API, Spark SQL, and (optionally) RDDs.

---

## Key Analyses Performed

- **Data Preprocessing**: Standardization, normalization, and handling missing data.
- **Trend Analysis**: Tracking efficiency metrics (e.g., TS%, PER) over multiple seasons.
- **Player Segmentation**: Classifying players into categories such as *Rookie*, *Role Player*, and *Star* based on stats.
- **Window Function Analysis**: Ranking players and computing rolling statistics by season.
- **Correlation Analysis**: Identifying relationships between playing time, experience, and performance metrics.
- **Anomaly Detection**: Finding outliers, such as players with extremely high minutes played.
- **Performance Comparison of PySpark APIs**: Benchmarking DataFrame API, Spark SQL, and RDDs.

---

## Example Insights

- **True Shooting Percentage** is the most stable and reliable indicator of efficiency over time.
- **Player Segmentation** revealed that Stars significantly differ in PER and WS compared to other roles.
- **High correlation** found between minutes played and games played, as well as between rebounding metrics.
- **Anomalies**: Very few detected (~0.02%), mostly due to outliers in minutes played.
- **Performance**: DataFrame API was the most efficient, followed closely by Spark SQL. RDDs performed the worst.

---

## Setup & Installation

### Requirements

- Python 3.9+
- PySpark 3.5+
- Jupyter Notebook or Google Colab

### Run the Notebook

```bash
pip install pyspark
jupyter notebook
