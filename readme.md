
# Dimensionality Reduction for Breast Cancer Diagnosis

## **Project Context**
This project is a continuation of the previous work, [Breast Cancer Diagnosis: Feature Importance and Model Comparison](https://github.com/puigdedios/Breast-Cancer-Diagnosis-Feature-Importance-and-Model-Comparison.git), where we analyzed the Breast Cancer Wisconsin dataset to identify the most important features for tumor classification. 

Building on those insights, this project focuses on dimensionality reduction:
1. **From Feature Importance to Feature Selection**: We leverage the feature importance rankings from the previous project to identify the top predictive features.
2. **From Visualization to Efficiency**: Principal Component Analysis (PCA), previously used for visualization, is now applied for dimensionality reduction in model training.

This project demonstrates how to optimize diagnostic models by reducing complexity while maintaining high performance.

---

## **Project Overview**
This project explores dimensionality reduction techniques on the Breast Cancer Wisconsin (Diagnostic) dataset to build a compact diagnostic model without sacrificing prediction performance. The primary objectives are:
1. Reduce the dataset dimensionality using **PCA** and **feature selection**.
2. Train models on the reduced datasets and compare their performance with the baseline model trained on the full feature set.
3. Identify the most critical features for breast cancer diagnosis.

---

## **Dataset**
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))
- **Description**: 
  - The dataset contains 569 samples of tumor cell nuclei measurements.
  - Features: 30 numerical attributes describing cell characteristics.
  - Target Variable: Diagnosis (`M` for Malignant, `B` for Benign).

---

## **Techniques Explored**
1. **Baseline Model**:
   - Trained a Random Forest Classifier using all 30 features as the benchmark.
2. **Principal Component Analysis (PCA)**:
   - Reduced the dataset dimensions to retain 95% of variance.
   - Trained a model on the PCA-reduced dataset.
3. **Feature Selection**:
   - Used Random Forest feature importance scores to select the top 10 most predictive features.
   - Trained a model using only these selected features.

---

## **Results Summary**
1. **Baseline Model**:
   - Accuracy: **96%**
   - Trained on all 30 features.
2. **PCA-Reduced Features**:
   - Accuracy: **95%**
   - Slight trade-off in performance but computationally efficient.
3. **Selected Features (Top 10)**:
   - Accuracy: **96%**
   - Matches baseline performance with fewer features, making it ideal for a compact diagnostic model.

---

## **Technologies Used**
- **Programming Language**: Python
- **Libraries**:
  - Data Manipulation: `pandas`, `numpy`
  - Machine Learning: `scikit-learn`
  - Visualization: `matplotlib`

---


## **How to See Results**
To view the analysis and results, open the file dimensionality_reduction_for_breast_cancer_diagnosis.ipynb, which is listed in the repository's file list above.
   

---

## **Deliverables**
1. **Compact Diagnostic Model**:
   - A model trained on the top 10 selected features, achieving 96% accuracy.
2. **Visualizations**:
   - Feature importance bar plots.
   - PCA variance explained.
3. **Detailed Code Explanation**:
   - See [code_explanation.md](./code_explanation.md) for a comprehensive walkthrough.

---

## **Acknowledgments**
- UCI Machine Learning Repository for providing the dataset.
- scikit-learn for versatile machine learning tools.

---

## **Contact**
For questions or collaboration, reach out at:
- **Email**: puigdedios@gmail.com
