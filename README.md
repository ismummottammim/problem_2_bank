# problem_2_bank
# Problem Set 02 - Bank Marketing Analysis

## Objective
Predict whether a client will subscribe to a term deposit (`y`) using the Bank Marketing dataset.

## Dataset
- **File**: `bank-full.csv`
- **Rows**: ~45,000
- **Columns**: 17 features (numerical + categorical)
- **Target Variable**: `y` (yes/no)

## Methodology
1. **Exploratory Data Analysis (EDA)**
   - Checked target distribution
   - Explored relationships of numerical and categorical features with target
   - Visualized important trends

2. **Data Preprocessing**
   - Encoded target (`yes` → 1, `no` → 0)
   - Label encoded categorical features
   - Standardized numerical features

3. **Model Training**
   - Logistic Regression with `class_weight='balanced'` to handle class imbalance
   - Train-test split: 80%-20%
   - Scaled features using StandardScaler

4. **Model Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC
   - Confusion Matrix and ROC Curve visualizations
   - Feature importance analysis using logistic regression coefficients

## Key Findings
- **Strongest Predictors**:
  - `duration` (call duration)
  - `poutcome` (previous campaign outcome)
- Model Metrics:
  - Test Accuracy: 80.94%
  - ROC-AUC: 0.8762
  - Accuracy  : 0.8094 (80.94%)
Precision : 0.3590
Recall    : 0.8015
F1 Score  : 0.4959

- The model captures the imbalance using class weighting effectively.
