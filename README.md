# Experiment-9
# Experiment No. 12: Data Preprocessing and Handling Missing Values

## Student Details

**Name:** Aanjneya Pankharaj
**PRN:** 25070123002
**Batch:** ENTC A1

---

## Overview

This experiment demonstrates the process of data preprocessing using Python. It focuses on identifying, handling, and treating missing values in datasets, along with standardising and cleaning the data for further analysis.

Two datasets are used in this experiment:

* A manually created student dataset
* The Cars93 dataset

---

## Objectives

* To understand the importance of data preprocessing
* To detect missing values in datasets
* To apply techniques such as removal and imputation
* To convert and standardise data formats
* To prepare clean datasets for analysis

---

## Tools and Libraries Used

* Python
* Pandas
* NumPy

---

## Key Steps Performed

### 1. Creation of Sample Dataset

A DataFrame was created with intentional missing values using NumPy (`np.nan`) to simulate real-world data issues.

### 2. Detection of Missing Values

* Used `isna()` and `notna()` functions
* Counted missing values column-wise using `sum()`

### 3. Handling Missing Values

* Removed rows with missing values using `dropna()`
* Replaced missing values with:

  * Constant values
  * Mean (for numerical columns like Age)
  * Median (for numerical columns like Marks)
  * Mode (for categorical columns like AirBags)

### 4. Data Cleaning

* Replaced invalid entries (e.g., '-') with `NaN`
* Converted columns to appropriate numeric types using `pd.to_numeric()`
* Standardised text data (e.g., department names to uppercase)

### 5. Date Formatting

* Converted date column into proper datetime format using `pd.to_datetime()`

### 6. Processing Second Dataset (Cars93)

* Identified missing values in columns
* Filled missing values as follows:

  * Luggage.room → Mean
  * Rear.seat.room → Mean
  * AirBags → Mode

### 7. Saving Cleaned Data

Exported cleaned datasets to CSV files:

* `cleaned_student_data.csv`
* `cleaned_Cars93.csv`

---

## Results

* All missing values were successfully handled
* Data was cleaned and standardised
* Final datasets contained no null values
* Cleaned datasets were stored for future analysis

---

## Conclusion

The experiment effectively demonstrated the significance of preprocessing in data analysis. Handling missing values and correcting inconsistencies ensured that the datasets became reliable and analysis-ready. Proper preprocessing improves the accuracy of any further analytical or machine learning tasks.

---

## Files Generated

* `data.csv`
* `cleaned_student_data.csv`
* `cleaned_Cars93.csv`
