## Credit Policy Analysis & Machine Learning Modeling

This project focuses on credit policy analysis using historical loan data.
The main objective is to understand portfolio performance over time, engineer stable and interpretable features, and train machine learning models to support credit decision-making.

The analysis combines risk analytics best practices with modern ML interpretability techniques.

### 1️. Vintage Analysis

Evaluation of credit performance by origination cohort.

Objectives:

Track default behavior over time

Identify deterioration or improvement in credit quality

Validate policy changes across vintages

Key outputs:

Default rate evolution by vintage

Cohort-level performance comparison

### 2. Feature Engineering

Feature engineering is designed to ensure model stability, robustness, and interpretability.

- Population Stability Index (PSI)

PSI is used to:

Measure feature drift between training and validation samples

Detect unstable or shifted variables

Exclude features with excessive population drift

Typical thresholds:

PSI < 0.1 → Stable

0.1 ≤ PSI < 0.25 → Monitor

PSI ≥ 0.25 → Unstable (excluded)

- Variance Inflation Factor (VIF)

VIF is used to:

Detect multicollinearity

Remove redundant features

Improve model interpretability and numerical stability

### 3️. Machine Learning Models

Several machine learning models are trained and evaluated, including:

Logistic Regression (baseline & interpretable)

Tree-based models (e.g. Random Forest, Gradient Boosting)

Evaluation metrics:

AUC / ROC

Precision / Recall

Models are trained using time-aware validation to avoid look-ahead bias.

### 4. Model Explainability with SHAP

SHAP (SHapley Additive exPlanations) is used to ensure transparent and explainable credit decisions.

Use cases:

Global feature importance

Directionality of risk drivers

Individual prediction explanations

SHAP outputs support:

Regulatory explainability

Business understanding

Credit policy discussions
