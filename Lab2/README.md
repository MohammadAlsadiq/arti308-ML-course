# Lab 2: Identifying ML Problems, Selecting Open Datasets, and Drawing a Methodology Diagram

**Course:** ARTI 308 – Machine Learning  
**Term:** Academic Year (2025/2026) – 1st Semester  

---

## 1. Problem Definition & Formulation

### Problem Statement
The goal of this project is to construct a predictive model that estimates residential property sale prices based on physical architectural characteristics and surrounding community indicators (including square footage, number of bedrooms/bathrooms, lot size, construction year, school ratings, and localized crime rates). Accurately predicting market values assists buyers, sellers, and financial lenders in establishing objective valuations.

### Machine Learning Task
* **Paradigm:** Supervised Learning 
* **Task Type:** Regression 
* **Justification:** The expected output is a continuous, numerical valuation (price in USD), rather than discrete categorical labels or unsupervised clusters .

### Target & Feature Space
* **Target Variable ($y$):** `Price` (Continuous integer representing property market value) .
* **Predictor Features ($X$):**
  * `Bedrooms` (Count)
  * `Bathrooms` (Count / Ratio)
  * `SquareFeet` (Living area size)
  * `YearBuilt` (Construction year)
  * `GarageSpaces` (Vehicle capacity)
  * `LotSize` (Property acreage / dimensions)
  * `CrimeRate` (Regional safety index)
  * `SchoolRating` (Educational district metric)

---

## 2. Dataset Overview

* **Source Platform:** Kaggle Open Datasets (Tabular CSV) 
* **Structure:** Tabular dataset containing 300 instances and 9 features (300 × 9) .
* **Data Integrity:** All columns are numeric (`int64`, `float64`) with 0 missing values across the entire dataset.

---

## 3. Methodology Diagram

Below is the structured machine learning workflow illustrating the end-to-end execution pipeline from raw data to evaluation :

![Methodology Diagram](methodology_diagram.png)

*(Diagram designed and generated via Draw.io / XML workflow specification )*

---

## 4. Repository Structure

```text
lab2/
│── lab2.ipynb                 # Jupyter Notebook with data loading & inspection (.shape, .head(), .info())
│── USA_Housing_kaggle.csv            # Tabular dataset used for the assignment
│── methodology_diagram.png    # Exported methodology flowchart
└── README.md                  # Problem definition and project documentation