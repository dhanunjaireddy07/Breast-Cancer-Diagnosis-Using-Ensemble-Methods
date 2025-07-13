# Breast-Cancer-Diagnosis-Using-Ensemble-Methods


# 🔬 Innovative Methods for Breast Cancer Diagnosis

## 📌 Project Overview
This project presents an optimized pipeline for **breast cancer classification** using advanced **dimensionality reduction techniques** and **machine learning models**. The goal is to improve diagnostic accuracy by reducing data complexity and leveraging powerful classifiers and ensemble methods. The Wisconsin Breast Cancer Diagnostic Dataset (WBCD) was used for evaluation.

## 🧠 Motivation
Breast cancer is among the most prevalent and deadly cancers affecting women globally. Early and accurate diagnosis is crucial to improving survival rates. Traditional techniques like PCA combined with basic neural networks are limited by linear assumptions and small datasets. This project addresses these challenges by:
- Using **Kernel PCA (RBF)** and **Autoencoders** to capture non-linear relationships.
- Applying advanced classifiers like **SVM** and **MLP**.
- Enhancing performance through **ensemble learning** (Soft Voting & Stacking).
- Evaluating using **precision**, **recall**, **F1-score**, and **ROC-AUC**, not just accuracy.

## 📂 Features
- Non-linear **dimensionality reduction** with Kernel PCA (RBF Kernel)
- **Multilayer Perceptron (MLP)** with ReLU & Adam optimizer
- **Support Vector Machine (SVM)** with grid search tuning
- **Soft Voting Ensemble** combining SVM, MLP, Random Forest, and XGBoost
- **Stacking Ensemble** with Logistic Regression meta-model
- Evaluation using **cross-validation**, **confusion matrix**, **ROC-AUC**, etc.

## 📁 Project Structure
```
BreastCancerDiagnosis/
│
├── data/                       # Wisconsin Breast Cancer Dataset (WBCD)
├── models/                    # Trained model files (SVM, MLP, Ensembles)
├── src/
│   ├── preprocessing.py       # Standardization, PCA/KPCA
│   ├── models.py              # ML model building
│   ├── train.py               # Training pipeline
│   └── evaluation.py          # Performance metrics
├── results/                   # ROC curves, confusion matrices
├── README.md                  # Project documentation
```

### 📊 View Evaluation Metrics
Output includes:
- Accuracy
- Precision / Recall / F1-score
- ROC-AUC
- Confusion Matrix

## 📊 Dataset Details
- **Dataset**: [Wisconsin Breast Cancer Diagnostic Dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))
- **Instances**: 569
- **Features**: 30 real-valued input features
- **Target**: Malignant (M), Benign (B)

## ✅ Evaluation Metrics
- **Cross-Validation Accuracy**
- **Precision & Recall**
- **F1-Score**
- **ROC Curve and AUC**
- **Confusion Matrix**

## 🧠 Models Used
- SVM with RBF Kernel
- MLP (Neural Network)
- Soft Voting Ensemble (SVM, MLP, RF, XGBoost)
- Stacking Ensemble (Base: SVM, MLP, RF, GB; Meta: Logistic Regression)

## 📊 Results Summary
| Model                     | Accuracy | ROC AUC | Highlights                        |
|--------------------------|----------|---------|----------------------------------|
| SVM                      | ~91%     | 0.985   | Strong precision, moderate recall |
| MLP                      | ~94%     | 0.986   | High recall and stable output     |
| Soft Voting Ensemble     | ~95.6%   | 0.990   | Best for recall-heavy situations  |
| Stacking Ensemble        | ~95.6%   | 0.993   | Best overall performance          |


