# Gear Fault Detection

## Overview
A machine learning project designed to detect gearbox faults using sensor data acquired via LabVIEW. It features a complete pipeline from raw data acquisition in both normal and malfunctioning settings, to feature extraction, and finally predictive modeling using Support Vector Classifier (SVC) and Random Forest algorithms to ensure robust fault detection.

## Features
* **Data Acquisition:** Leveraged LabVIEW to acquire high-resolution sensor data capturing both normal and faulty gearbox behavior.
* **Feature Engineering:** Extracted 24 key features from raw sensor data, including frequency-domain metrics.
* **Machine Learning:** Implemented scikit-learn to train and evaluate Support Vector Classifier (SVC) and Random Forest (RFC) models.
* **Model Optimization:** Improved model accuracy from a 50% baseline to over 82% through rigorous feature selection and dimension reduction techniques.

---

## System & Data Overview

### Gear Conditions
| Normal Gear | Faulty Gear |
|:---:|:---:|
| <img src="https://github.com/user-attachments/assets/cac75302-5745-4a3b-b64e-23e8586b8fe3" width="300" height="300"> | <img src="https://github.com/user-attachments/assets/b46bf5d0-07b2-4210-8f72-2691635fe22c" width="300" height="300"> |

### Raw Sensor Data
**Array Shape:** `(10, 51200, 2)` for both Normal and Faulty sets.

| Normal Data | Faulty Data |
|:---:|:---:|
| <img src="https://github.com/user-attachments/assets/25502d6c-c23f-414a-a6cb-3918178464a5" width="400" height="400"> | <img src="https://github.com/user-attachments/assets/1c14cb46-a72d-485d-b301-63bd082cc519" width="400" height="400"> |

---

## Results & Optimization

**Extracted Features Array Shape:** `(10, 24)`
<br>
<img src="https://github.com/user-attachments/assets/57c4f1ab-7ace-4fdb-80c8-fcbca7175f53" width="350" height="600">

### 1. Baseline Model Performance
Initial testing for both SVC and RFC yielded the following baseline metrics:
* **Accuracy:** 50.00%
* **Precision:** 50.00%
* **Recall:** 100.00%

### 2. Feature Selection
By isolating the **Top 5 Features** (*Sum Freq, Var Freq, Max Freq, Kurtosis Freq, Peak Freq*), model accuracy improved significantly:
* **Random Forest (RFC):** 74.66%
* **Support Vector Classifier (SVC):** 78.00%

<img src="https://github.com/user-attachments/assets/658ec375-8bdf-4078-82c6-600e6b40799e" width="300" height="400">

### 3. Dimension Reduction (Final Results)
Applying dimension reduction techniques yielded the highest overall performance:
* **Random Forest (RFC):** 78.20%
* **Support Vector Classifier (SVC):** 82.77%
