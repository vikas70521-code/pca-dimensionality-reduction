# PCA for Dimensionality Reduction

This project demonstrates **Principal Component Analysis (PCA)** for reducing the dimensionality of the **Breast Cancer Wisconsin dataset**.

The project investigates how PCA can reduce the number of features while retaining most of the information in the dataset. Logistic Regression is used to compare model performance before and after dimensionality reduction.

## Objective

* Understand the working of PCA
* Standardize features before applying PCA
* Determine the number of components required to retain approximately 95% variance
* Compare Logistic Regression performance before and after PCA
* Build a Scikit-learn Pipeline
* Evaluate the model using 5-fold cross-validation

## Dataset

The project uses the Breast Cancer Wisconsin dataset available through Scikit-learn.

* Samples: 569
* Original features: 30
* Target: Binary classification

## Workflow

1. Load the dataset
2. Understand the dataset
3. Perform exploratory data analysis
4. Split the data into training and testing sets
5. Standardize the features using `StandardScaler`
6. Apply PCA
7. Analyze explained variance
8. Select components retaining approximately 95% variance
9. Visualize the principal components
10. Train Logistic Regression before PCA
11. Train Logistic Regression after PCA
12. Build a Scikit-learn Pipeline
13. Perform 5-fold cross-validation
14. Compare the results

## Results

| Metric                   | Result |
| ------------------------ | -----: |
| Original Features        |     30 |
| PCA Components           |     10 |
| Dimensionality Reduction | 66.67% |
| Variance Retained        |   ~95% |
| Accuracy Without PCA     |    98% |
| Accuracy With PCA        |    97% |
| Mean 5-Fold CV Accuracy  |   ~98% |

## Key Learning

PCA reduced the dataset from **30 features to 10 principal components**, resulting in a **66.67% reduction in dimensionality** while retaining approximately **95% of the variance**.

Logistic Regression accuracy decreased slightly from approximately **98% to 97%** after PCA. This demonstrates the trade-off between dimensionality reduction and predictive performance.

The project also demonstrates how Scikit-learn's `Pipeline` can combine preprocessing, PCA, and model training into a single workflow.

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook / Google Colab

## Project Structure

```text
pca-dimensionality-reduction/
│
├── PCA_Dimensionality_Reduction.ipynb
├── README.md
└── requirements.txt
```

## How to Run

Clone the repository and open the notebook in Jupyter Notebook or Google Colab.

Install the required libraries:

```bash
pip install -r requirements.txt
```

Then open:

```text
PCA_Dimensionality_Reduction.ipynb
```
