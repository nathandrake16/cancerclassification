# Cancer Type Classification Using Clinical and Gene Expression Data

This project focuses on predicting **cancer type** using a combination of **clinical information** and **gene expression profiles**. The dataset contains **seven cancer types**:

- COAD
- ESCA
- HNSC
- LIHC
- LUAD
- LUSC
- STAD

Both **clinical.csv** and **gene_expression.csv** files are provided for each cancer type.

---

## 🚀 Project Objectives
- Merge clinical and gene expression data across all cancer types.
- Reduce the high-dimensional gene expression features using **Principal Component Analysis (PCA)**.
- Train and evaluate machine learning models to classify cancer type.
- Ensure fair evaluation through **stratified train-test splitting** and **cross-validation**.

---

## 🧠 Methodology

### 1. Data Preparation
- Loaded and inspected clinical and gene expression data per cancer type.
- Identified and aligned common patient identifiers.
- Applied **PCA** to gene expression datasets to retain **95% variance** while reducing dimensionality.

### 2. Feature Integration
- Combined reduced PCA gene components with clinical features.
- Encoded categorical clinical data using **One-Hot Encoding**.

### 3. Model Training
Models used:
| Model | Purpose |
|-------|---------|
| Multinomial Logistic Regression | Baseline linear classifier |
| Random Forest Classifier | Non-linear classifier to capture complex patterns |

- Stratified **train-test split** ensures balanced representation.
- **5-Fold Stratified Cross-Validation** used for stable evaluation.

---

## 📊 Evaluation Metrics
Performance is measured using:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix Visualization

---

## 🖥️ Tech Stack
| Component | Tools Used |
|----------|------------|
| Language | Python |
| Libraries | pandas, numpy, scikit-learn, matplotlib, seaborn |
| Dimensionality Reduction | PCA (sklearn) |
| Models | Logistic Regression, Random Forest |

---

