
# Breast Cancer Diagnostic Classification & Risk Analysis

An interactive **machine learning and healthcare analytics portfolio project** focused on breast cancer diagnostic classification and risk analysis.

The project explores differences between malignant and benign tumor characteristics, evaluates machine learning classification models, and visualizes diagnostic performance through an interactive dashboard.

**Technologies:** HTML, CSS, JavaScript, D3.js, Machine Learning, Data Visualization

## Live Interactive Dashboard

[View Breast Cancer Diagnostic Dashboard](https://urmillachowdary-bit.github.io/Breast-Cancer-Diagnostic-Classification-and-Risk-Analysis/)

*The dashboard is accessible after GitHub Pages has been enabled and successfully deployed.*

---

## Dashboard Preview

![Breast Cancer Diagnostic Classification Dashboard](breast-cancer.png)

The interactive dashboard includes tumor feature analysis, machine learning model comparisons, ROC curves, confusion matrices, and classification threshold controls.

---

## Project Overview

This project analyzes the **Wisconsin Diagnostic Breast Cancer (WDBC) dataset** to investigate differences between malignant and benign tumor measurements.

The dataset contains 569 tumor samples and 30 numerical features derived from digitized fine-needle aspirate images of breast masses.

The primary objective is to evaluate classification algorithms and explore how tumor characteristics contribute to malignancy prediction.

### Project Objectives

- Analyze tumor measurements to distinguish malignant and benign samples.
- Compare multiple machine learning classification models.
- Evaluate predictive performance using classification metrics.
- Identify important tumor characteristics associated with malignancy.
- Examine false-positive and false-negative predictions.
- Explore how decision thresholds influence malignant-case detection.
- Communicate findings through interactive visualizations.

---

## Dataset Information

**Dataset:** Wisconsin Diagnostic Breast Cancer (WDBC)

**Source:** UCI Machine Learning Repository

| Dataset Characteristic | Value |
|---|---|
| Total Samples | 569 |
| Malignant Tumors | 212 |
| Benign Tumors | 357 |
| Total Features | 30 |
| Target Variable | Diagnosis (Malignant / Benign) |
| Training/Test Split | 80% / 20% |
| Held-Out Test Samples | 114 |
| Malignant Samples in Test Set | 42 |

The 30 features describe characteristics of cell nuclei, including radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension.

---

## Machine Learning Models

The dashboard compares four classification algorithms:

1. **Logistic Regression**
   - A linear classification model used to estimate the probability of malignancy.

2. **Random Forest**
   - An ensemble learning algorithm combining multiple decision trees.

3. **Support Vector Machine (SVM)**
   - A classification algorithm that identifies a separating decision boundary between tumor classes.

4. **K-Nearest Neighbors (KNN)**
   - A distance-based classification algorithm that predicts classes using neighboring samples.

Model performance is evaluated using held-out predictions and reported cross-validation results.

---

## Key Results

| Performance Metric | Reported Result |
|---|---|
| Total Tumor Samples | 569 |
| Best Test Accuracy | **98.2%** |
| Best Accuracy Model | Support Vector Machine (SVM) |
| Correctly Classified Test Samples | 112 of 114 |
| Malignant Recall (SVM) | **95.2%** |
| Malignant Tumors Correctly Identified | 40 of 42 |
| Missed Malignant Cases | 2 |
| Best Test ROC-AUC | **0.996** |
| Models With Best Reported ROC-AUC | Logistic Regression and SVM |

### Key Finding

The Support Vector Machine achieved **98.2% classification accuracy** on the held-out test data and identified **95.2% of malignant samples** at the default classification threshold.

However, two malignant samples were incorrectly classified. This highlights the importance of evaluating recall and false-negative predictions rather than relying on accuracy alone.

These findings are specific to the benchmark dataset and do not establish clinical diagnostic effectiveness.

---

## Dashboard Features

### 1. Tumor Feature Analysis

- Identifies tumor measurements that distinguish malignant and benign samples.
- Analyzes individual features using ROC-AUC.
- Compares distributions of malignant and benign tumor measurements.
- Provides interactive visualizations for exploring diagnostic characteristics.

### 2. Model Performance Comparison

The dashboard compares:

- Logistic Regression
- Random Forest
- Support Vector Machine
- K-Nearest Neighbors

Evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Cross-Validation Performance

### 3. ROC Curve Analysis

- Compares model discrimination performance.
- Visualizes true-positive and false-positive rates.
- Displays model performance across classification thresholds.

### 4. Confusion Matrix Analysis

- Displays true positives and true negatives.
- Identifies false-positive predictions.
- Highlights false-negative predictions involving missed malignant samples.
- Supports comparison between classification models.

### 5. Classification Threshold Analysis

The dashboard provides two threshold settings:

- Default classification threshold of 0.50.
- A training-derived threshold targeting 97% malignant recall.

Users can compare the effect of these settings on the classification of held-out tumor samples.

---

## Methodology

### Step 1: Data Preparation

The dashboard documents a machine learning workflow using 569 tumor samples with 30 numerical features.

### Step 2: Train-Test Split

An 80/20 stratified training and testing split was used in the documented evaluation.

### Step 3: Feature Scaling

StandardScaler was used in the described preprocessing pipeline to standardize numerical features.

### Step 4: Feature Selection

SelectKBest with an ANOVA F-test was used for feature selection.

### Step 5: Model Evaluation

Logistic Regression, Random Forest, SVM, and KNN were compared using classification metrics and ROC-AUC.

### Step 6: Hyperparameter Optimization

The documented workflow describes cross-validation-based model tuning and feature selection.

### Step 7: Threshold Analysis

Classification thresholds were evaluated to examine the trade-off between malignant recall and false-positive predictions.

**Reproducibility Note:** The repository provides the interactive dashboard with embedded data and prepared model predictions. The original Python model-training scripts are not included.

---

## Technologies Used

| Category | Technologies |
|---|---|
| Frontend Development | HTML5, CSS3, JavaScript |
| Data Visualization | D3.js, SVG |
| Documented Machine Learning | Logistic Regression, Random Forest, SVM, KNN |
| Data Preparation Methods | StandardScaler, SelectKBest |
| Model Evaluation | Accuracy, Precision, Recall, F1-Score, ROC-AUC |
| Diagnostic Analysis | Confusion Matrix, False Negatives, False Positives |
| Version Control | Git, GitHub |
| Deployment | GitHub Pages |

---

## Repository Structure

```text
Breast-Cancer-Diagnostic-Classification-and-Risk-Analysis/
│
├── index.html
├── README.md
└── breast-cancer.png
```

All files are located in the repository's root directory.

---

## How to Run the Project

1. Download the repository files.
2. Locate the `index.html` file.
3. Open `index.html` in Google Chrome, Microsoft Edge, or Firefox.
4. Explore the interactive breast cancer diagnostic dashboard.
5. Compare the machine learning models, tumor characteristics, and evaluation metrics.

No additional software installation, database connection, or build process is required.

---

## GitHub Pages Deployment

To publish the dashboard online:

1. Open the repository on GitHub.
2. Navigate to **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select the `main` branch.
5. Choose the `/(root)` folder.
6. Click **Save**.
7. After successful deployment, open the live dashboard link above.

---

## Data Source & Attribution

**Wisconsin Diagnostic Breast Cancer Dataset**

- Repository: UCI Machine Learning Repository
- Dataset: Breast Cancer Wisconsin (Diagnostic)
- Samples: 569
- Features: 30 numerical measurements
- Classification Labels: Malignant and Benign

**Dataset Link:**

https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic

The dashboard uses the D3.js visualization library. Third-party dataset and software licensing terms should be reviewed before redistribution.

---

## Project Limitations

- This project is intended for educational and portfolio demonstration purposes.
- It is not intended for medical diagnosis or treatment decisions.
- Reported model performance is specific to the Wisconsin Diagnostic Breast Cancer dataset.
- The original Python model-training scripts are not included.
- Performance on this dataset does not guarantee effectiveness in real-world clinical settings.
- Classification thresholds influence recall, precision, and diagnostic error rates.
- The project is implemented as an HTML/JavaScript dashboard rather than a native Power BI or Tableau workbook.

---

## Portfolio Relevance

This project demonstrates knowledge of:

- Healthcare data analytics
- Exploratory data analysis
- Machine learning classification
- Feature analysis and interpretation
- Model performance evaluation
- Diagnostic risk assessment
- Interactive data visualization
- Communicating analytical findings

The project is relevant to **Data Analyst, Healthcare Data Analyst, Business Intelligence Analyst, and entry-level Machine Learning Analyst** roles.
