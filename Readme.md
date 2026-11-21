# Seeds Dataset – Exploratory Data Analysis (EDA)

## Project Overview

This project performs **basic Exploratory Data Analysis (EDA)** on the UCI Seeds dataset. It explores measurements of wheat kernels from three different varieties using Python, NumPy, Pandas, and Matplotlib.

The dataset contains **210 rows (samples)** representing three wheat varieties.

**Dataset source:** [UCI Machine Learning Repository – Seeds Dataset](https://archive.ics.uci.edu/dataset/236/seeds)

## Project Objectives

The objectives are to inspect the dataset, summarize important kernel measurements, compare the three varieties, identify data-quality issues, and visualize the results.

## Questions to Explore

1. How many samples belong to each variety?
2. Calculate the mean, median, minimum, and maximum for kernel area, perimeter, and length.
3. Which variety has the highest average kernel area and width?
4. Sort the records by kernel area and show the top 10 samples.
5. Are there any missing values or duplicate records?
6. How do the average measurements compare across the three varieties?

## Tools and Libraries

- **Python** – Main programming language.
- **NumPy** – Numerical calculations and statistical analysis.
- **Pandas** – Data loading, inspection, filtering, sorting, and grouping.
- **Matplotlib** – Data visualization.

Install the required libraries using:

```bash
pip install -r requirements.txt
```

## Dataset Information

- **Dataset name:** Seeds
- **Source:** UCI Machine Learning Repository
- **Number of samples:** 210
- **Number of varieties:** 3
- **Data type:** Geometrical measurements of wheat kernels

The dataset contains measurements such as area, perimeter, compactness, kernel length, kernel width, asymmetry coefficient, and kernel groove length, along with a variety/class label.

## Project Tasks

### 1. Load and Inspect the Dataset

Load the Seeds dataset and display:

- `head()` – First five rows.
- `tail()` – Last five rows.
- `shape` – Number of rows and columns.
- `info()` – Column names, data types, and non-null counts.
- `describe()` – Descriptive statistical summary.

### 2. Variety Distribution

Use Pandas `value_counts()` to count the number of samples in each wheat variety.

### 3. Kernel Measurement Statistics

Use NumPy arrays to calculate the following statistics for each of these measurements:

- Kernel area
- Kernel perimeter
- Kernel length

Calculate the:

- Mean
- Median
- Minimum
- Maximum

### 4. Variety-wise Area and Width Comparison

Use Pandas `groupby()` to calculate average kernel area and average kernel width for each variety. Identify the variety with the highest average for each measurement.

### 5. Top 10 Samples by Kernel Area

Use Pandas `sort_values()` to sort records by kernel area in descending order and display the top 10 samples.

### 6. Data Quality Check

Check the dataset for:

- Missing values using `isnull().sum()`.
- Duplicate records using `duplicated().sum()`.

### 7. Compare Average Measurements

Group the data by variety and compare the average values of the available kernel measurements across all three varieties.

### 8. Data Visualization

Create the following two simple charts using Matplotlib:

1. **Variety-count bar chart** – Shows the number of samples in each wheat variety.
2. **Kernel-area histogram** – Shows the distribution of kernel area values.

## Common Requirements Checklist

- [ ] Use Python, NumPy, and Pandas.
- [ ] Load the Seeds dataset.
- [ ] Display `head()`, `tail()`, `shape`, `info()`, and `describe()`.
- [ ] Check missing values and duplicate records.
- [ ] Use at least one NumPy array for numerical calculations.
- [ ] Use Pandas `value_counts()`, `groupby()`, filtering, and `sort_values()` where relevant.
- [ ] Create a variety-count bar chart.
- [ ] Create a kernel-area histogram.
- [ ] Write three observations based on the analysis.

## Three Observations

After completing the analysis, write three observations supported by the results. For example:

1. State which wheat variety has the highest number of samples.
2. Identify which variety has the highest average kernel area and width.
3. Describe the distribution of kernel area and any differences observed between varieties.

**Note:** Fill in the actual findings after running the analysis. Do not assume the observations before checking the dataset.

## Project Scope

This project covers **basic EDA only**. It does not include machine learning, model training, prediction, or classification.

## How to Run the Project

1. Clone or download the project.
2. Open the project folder in VS Code or another Python editor.
3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the Python analysis file:

   ```bash
   python main.py
   ```

   Replace `main.py` with the actual Python filename if it is different.

5. Review the printed analysis, charts, and three observations.

## Conclusion

This project uses basic Python data-analysis tools to explore the UCI Seeds dataset, understand the distribution of wheat varieties, summarize kernel measurements, compare average measurements across varieties, check data quality, and present findings through simple visualizations.
