# Gear Fault Detection
Acquired sensor data in both working and malfunctioning settings leveraging LabView, guaranteeing thorough coverage of gearbox behavior. Extracted pertinent information from raw sensor data, using feature extraction techniques.	Implemented scikit-learn for model development and implemented machine learning algorithms to detect gearbox faults, such as Support Vector Classifier (SVC) and Random Forest. Ensured strong fault detection capabilities by assessing models' performance using metrics such as accuracy, precision, and recall.

## Figure
<p align="center">
  ![WhatsApp Image 2025-03-21 at 20 58 31_c472aabf](https://github.com/user-attachments/assets/e8097fdf-db07-4d28-bce6-cb8d1db99ba6)<br/>
  Figure 1 - Normal Gear<br/>
  ![WhatsApp Image 2025-03-21 at 20 58 32_5842191b](https://github.com/user-attachments/assets/b46bf5d0-07b2-4210-8f72-2691635fe22c)<br/>
  Figure 2 - Faulty Gear<br/>
  ![WhatsApp Image 2025-03-21 at 20 58 32_285a39a4](https://github.com/user-attachments/assets/6af9f748-55de-443d-8fb6-9ef5f7fdd59d)<br/>
  Figure 3 - Gear Box<br/>
</p>

## Results
Shape of Normal Data Array: (10, 51200, 2)

Shape of Faulty Data Array: (10, 51200, 2)

![WhatsApp Image 2025-01-01 at 13 59 26_fba48d53](https://github.com/user-attachments/assets/962592cb-a4b4-45db-a5a8-9eb18fec4c8e)

Shape of Normal Features Array: (10, 24)

Shape of Faulty Features Array: (10, 24)

![WhatsApp Image 2025-01-01 at 14 02 02_7d90b447](https://github.com/user-attachments/assets/57c4f1ab-7ace-4fdb-80c8-fcbca7175f53)

## Support Vector Classifier (SVC)
Accuracy in %: 50.00 

Recall score in %: 100.00 

Precision score in %: 50.00

## Random Forest Classifier (RFC)
Accuracy in %: 50.00 

Recall score in %: 100.00 

Precision score in %: 50.00

## Feature Selection using SVC
![WhatsApp Image 2025-01-01 at 14 05 27_f643985a](https://github.com/user-attachments/assets/658ec375-8bdf-4078-82c6-600e6b40799e)

## Top 5 Features 
  Sum Freq, Var Freq, Max Freq, Kurtosis Freq, Peak Freq

Accuracy - RFC : 74.66 %

Accuracy - SVC : 78.00 %

## Dimension Reduction

Accuracy - RFC : 78.20 %

Accuracy - SVC : 82.77 %
