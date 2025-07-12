#  Lung Cancer Diagnosis Using MRI and Random Forest

This project leverages machine learning (Random Forest) to diagnose lung cancer using MRI images. The model classifies tumors as **Benign** or **Malignant** with a confidence score, providing a fast and non-invasive second opinion tool for early detection.

---

##  Table of Contents

- [Overview](#overview)
- [Project Goals](#project-goals)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Performance](#model-performance)
- [Streamlit GUI](#streamlit-gui)
- [Questions & Notes (Q&N)]()


---

##  Overview

This is a machine learning-powered tool to help identify whether a lung tumor is **malignant** (cancerous) or **benign** using MRI images. It uses **feature extraction (HOG)** and a **Random Forest classifier**.

---

##  Project Goals

- Predict lung cancer from MRI scans using machine learning.
- Input: MRI image  
- Output: Diagnosis (Malignant/Benign) with confidence level  
- Accuracy target: ~90%
- GUI: Simple Streamlit interface for ease of use


---

## Technologies Used

- Python  
- Scikit-learn  
- OpenCV  
- Scikit-image (HOG)  
- Streamlit (GUI)  
- Matplotlib & Seaborn (for confusion matrix)

---

##  Installation



```bash
numpy
pandas
scikit-learn
opencv-python
scikit-image
matplotlib
seaborn
joblib
streamlit
Pillow
```
### Install dependencies:
````
!pip install -r requirements.txt

````
###  Usage

Upload an MRI image via the Streamlit web interface.

The model will predict if the tumor is malignant or benign.

You will also receive a confidence score (%).

A confusion matrix is generated in the notebook to assess accuracy.

###  Dataset

Source: Kaggle - The IQ-OTHNCCD lung cancer dataset

###  Model Performance

Classifier: Random Forest (n_estimators=200, max_depth=20)

Feature Extraction: HOG

Train-Test Split: 80/20

Accuracy: ~89–91%

###  Streamlit GUI

Upload an MRI image (JPG/PNG)

Get a real-time prediction

Confidence level shown

Warnings displayed for malignant cases

### Questions & Notes (Q&N) — Lung Cancer Diagnosis ML Project

######  Q1: What datasets were used?

A: MRI image dataset from Kaggle, categorized into benign and malignant folders. The dataset was manually verified, resized, and processed. Image labels were assumed accurate as per dataset metadata.

###### Q2: Why focus on lung cancer diagnosis using MRI images?

A: Lung cancer is one of the leading causes of cancer-related deaths worldwide. Early detection significantly improves treatment outcomes. MRI, while less commonly used than CT for lung imaging, provides non-invasive high-contrast imaging without radiation, making it suitable for repeated testing and detection of soft tissue changes.
