# Coding Task 

This repository contains my solution to a coding task focused on generating new data samples that resemble an original synthetic dataset.


## 1. Original Dataset Properties

Number of samples = 500
Columns:
- **Category1**: A categorical variable with values A–E with different probabilities.
- **Value1**: A continuous variable sampled from a normal distribution (mean ≈ 10, std ≈ 2).
- **Value2**: A continuous variable sampled from a normal distribution (mean ≈ 20, std ≈ 6).


## 2. Data Analysis with Analogy
Visualized the probability distributions of the categorical variable and histograms of the continuous variables of the dataset as a whole

Analogy - Bolts manufactured in a bolt manufacturing plant.

Category1  -->  Machine ID

Value1     -->  Length of bolts (in cm)

Value2     -->  Diameter of bolts (in mm)

Mapping to the analogy, continuous variables' descriptive statistics and their distributions per each categorical group, were analyzed

---

## 3. New Dataset Creation

Sample size - 2* original sample size

mean and the std of the continuous variables in categorical groups were calculated 

Data was generated for each Category1 value group and then concatenated to form the full dataset

---

## 4. Visual Comparison of the Distributions (Original vs New)

The similarity between the original and new datasets is validated through:
- **Bar plots** for categorical variable's probability distribution comparison.
- **KDE plots** for continuous variables' probability distribution.


---

## 5. Statistical Tests

To confirm similarity between the datasets, the following statistical tests are used:
- **Chi-Square Test** for checking the similarity of the distributions of the categorical variable
- **Kolmogorov-Smirnov (K-S) Test** for checking the similarity of the distributions of Value1 and Value2 accross datasets.
- H0- Distributions of the two samples are same. H1- Distributions of the samples are significantly different

## Results
Code was run and the results are integrated in the last section of the jupyter notebook, coding_task.ipynb.

---

## Libraries Used

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scipy`

---

## Files in the Repository

- `coding_task.ipynb` – Jupyter notebook with code, analysis, and plots.
- `dataset.csv` – The original dataset.
- `newdataset.csv` – The newly generated dataset.
- `README.md` – This file.

---

Author - Jeevanthi Panawala

