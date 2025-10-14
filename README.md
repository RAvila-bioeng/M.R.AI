# M.R.AI
Prediction of Alzheimer's desease using image recognition

# Alzheimer's Disease Detection and Classification using Neuroimaging (MRI) and Artificial Intelligence

## Academic and Institutional Framework

**MRI Image Classification Project for Alzheimer's Detection**

* **Institution:** Universidad Francisco de Vitoria (UFV)
* **Course:** Biomedical Image Processing with Artificial Intelligence
* **Professor:** Alberto de Santos
* **Context:** Biomedical Engineering
* **Course/Date:** December 2025
* **Repository URL:** [https://github.com/RAvila-bioeng/M.R.AI]

---

## Project Goal

The main goal of this project is to develop a robust and, critically, **interpretable Deep Learning** model for the automated classification of cerebral Magnetic Resonance Imaging (MRI) scans. The aim is to distinguish between healthy subjects (Normal Control, NC) and patients with different stages of Alzheimer's Disease (AD, MCI).

### Specific Objectives

1. **Short Term:** Implement a complete neuroimaging preprocessing *pipeline* (registration, normalization, etc.) and train a baseline Convolutional Neural Network (CNN).
2. **Medium Term:** Optimize the model architecture (e.g., 3D CNN, Transfer Learning) and achieve performance metrics that surpass academic *benchmarks* (e.g., Accuracy > 88%).
3. **Long Term:** Integrate **Explainability (XAI)** techniques such as Grad-CAM, LIME, or SHAP to justify the classification and visualize the cerebral regions of greatest diagnostic relevance.

---

## Problem Description

**Alzheimer's Disease (AD)** is the most common cause of dementia, characterized by progressive cognitive decline. Early diagnosis is crucial for clinical management and the initiation of treatments. This project addresses the challenge of early detection and classification through the analysis of structural neuroimaging (MRI), which can reveal cerebral atrophy, especially in the hippocampus and cortex.

**Clinical Relevance:** An AI-based decision support system can assist radiologists and neurologists in improving the **objectivity** and **efficiency** of diagnosis, minimizing inter-observer variability.

---

## Technology Stack

| Category | Tools/Libraries | Purpose |
| :--- | :--- | :--- |
| **Deep Learning** | TensorFlow, Keras, PyTorch | Development and training of CNN models. |
| **Neuroimaging** | nibabel, SimpleITK | Reading, writing, and manipulation of MRI files (NIfTI). |
| **Explainability (XAI)** | LIME, SHAP, Grad-CAM | Model interpretability to justify decisions. |
| **Data Science** | NumPy, Pandas, Scikit-learn | Data preprocessing, metrics, and validation. |
| **Environment** | Python 3.11, Conda/Pip | Dependency management. |

---

## Scientific Methodology (CRISP-DM Pipeline)

The project development follows a scientific and reproducible approach:

1. **Business/Clinical Understanding:** Definition of the Alzheimer's problem, selection of biomarkers, and clinically relevant metrics.
2. **Data Understanding:** Exploration of the *Dataset* (e.g., ADNI, OASIS, or Kaggle). Analysis of image quality, class distribution, and format.
3. **Data Preparation:**
    * Preprocessing: Format conversion, **registration**, and **normalization** to a standard *template* (e.g., MNI).
    * *Data Augmentation* to improve model robustness.
4. **Modeling:** Design and implementation of the Deep Learning architecture (e.g., adapted 3D CNN).
5. **Evaluation:** Rigorous validation with specific metrics and **Cross-Validation**.
6. **Deployment/Communication:** Documentation, GitHub repository, and demonstration of the model and its explanations.

---

## Clinical Evaluation Metrics

Evaluation is not limited to accuracy, but focuses on **diagnostic rigor** and clinical implications:

* **Accuracy:** [Goal: 88-95%] - Proportion of correct predictions.
* **Sensitivity (Recall):** [Goal: > 85%] - Ability to correctly identify sick patients (avoiding False Negatives). **Crucial for early *screening*.**
* **Specificity:** [Goal: > 90%] - Ability to correctly identify healthy subjects (avoiding False Positives).
* **AUC (Area Under the Curve):** [Goal: > 0.92] - Measure of discrimination between classes.

---

## Interpretability and Explainability (XAI)

Given the medical application, interpretability is fundamental. The following techniques will be implemented:

* **Grad-CAM:** Generation of **Activation Maps** superimposed on the original MRI images, highlighting the cerebral regions (e.g., hippocampus) the model considered most relevant for classification.
* **LIME (Local Interpretable Model-agnostic Explanations):** Providing explanations for individual (local) predictions.
* **SHAP (SHapley Additive exPlanations):** Analysis of the contribution of different features or regions to the final decision.

---

## Installation and Usage

### 1. Clone the Repository

```bash
git clone [[https://github.com/RAvila-bioeng/M.R.AI](https://github.com/RAvila-bioeng/M.R.AI)]
cd M.R.AI
