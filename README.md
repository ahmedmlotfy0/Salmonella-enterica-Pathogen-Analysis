# 🧬 Salmonella Enterica Pathogen Analysis

## 📌 Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on a large dataset of *Salmonella enterica* pathogen records. The goal is to process raw detection data, clean it, and uncover temporal trends and seasonal patterns in infection cases using Python.

This analysis bridges the gap between **Veterinary Medicine** and **Data Analytics**, applying technical data manipulation skills to biological data.

## 📂 Dataset
* **Source File:** `Pathogen detection Salmonella enterica.csv`
* **Size:** ~558,819 records
* **Key Features:**
    * **Metadata:** Strain, BioSample, Assembly, Location, Isolation Source.
    * **Pathogen Details:** Serovar, SNP Cluster, AMR Genotypes, Computed Types.
    * **Time:** Create Date.

## 🛠️ Technologies & Libraries
The project is implemented in **Python 3** using the following libraries:
* **Pandas:** Data manipulation and cleaning.
* **NumPy:** Numerical operations.
* **Matplotlib & Seaborn:** Data visualization (Time-series & Bar charts).
* **Re (Regular Expressions):** Text parsing for Serotype and Antigen extraction.

## ⚙️ Workflow & Methodology

### 1. Data Preprocessing
* **Date Standardization:** Converted `Create date` to datetime objects.
* **Feature Engineering:** Extracted `Year` and `Month` columns for temporal analysis.
* **Text Parsing (Regex):**
    * Extracted `antigen_formula` from the *Computed types* column.
    * Extracted `serotype` information using complex pattern matching.

### 2. Exploratory Data Analysis (EDA)
* **Trend Analysis:** Visualized the number of Salmonella isolates over the years to track long-term prevalence.
* **Seasonality:** Analyzed monthly distribution to identify seasonal spikes in infections.

## 📊 Key Findings
* **Temporal Trends:** Observed how the detection rate of *Salmonella enterica* has changed over the analyzed years.
* **Seasonality:** Identified specific months where case reporting is significantly higher.

## 🚀 How to Run
1. Clone this repository.
2. Ensure you have the required libraries installed:
   ```bash
   pip install pandas numpy matplotlib seaborn
