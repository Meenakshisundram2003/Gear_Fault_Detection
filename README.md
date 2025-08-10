# Gear Fault Detection
Acquired sensor data in both working and malfunctioning settings leveraging LabView, guaranteeing thorough coverage of gearbox behavior. Extracted pertinent information from raw sensor data, using feature extraction techniques.	Implemented sci-kit-learn for model development and implemented machine learning algorithms to detect gearbox faults, such as Support Vector Classifier (SVC) and Random Forest. Ensured strong fault detection capabilities by assessing models' performance using metrics such as accuracy, precision, and recall.

## Figure
| Normal Gear | Faulty Gear |
|-------------|-------------|
| <img src="https://github.com/user-attachments/assets/cac75302-5745-4a3b-b64e-23e8586b8fe3" width="400" height="400"> | <img src="https://github.com/user-attachments/assets/b46bf5d0-07b2-4210-8f72-2691635fe22c" width="400" height="400"> |

             
## Plots
Shape of Normal Data Array: (10, 51200, 2) <br/>
Shape of Faulty Data Array: (10, 51200, 2)<br/>

| Normal Data | Faulty Data |
|-------------|-------------|
| <img src="https://github.com/user-attachments/assets/25502d6c-c23f-414a-a6cb-3918178464a5" width="400" height="400"> | <img src="https://github.com/user-attachments/assets/1c14cb46-a72d-485d-b301-63bd082cc519" width="400" height="400"> |

## Results
Shape of Normal Features Array: (10, 24)<br/>
Shape of Faulty Features Array: (10, 24)<br/>

<img src="https://github.com/user-attachments/assets/57c4f1ab-7ace-4fdb-80c8-fcbca7175f53" width="400" height="700">


## Support Vector Classifier (SVC)
Accuracy in %: 50.00 <br/>
Recall score in %: 100.00 <br/>
Precision score in %: 50.00

## Random Forest Classifier (RFC)
Accuracy in %: 50.00 <br/>
Recall score in %: 100.00 <br/> 
Precision score in %: 50.00

## Feature Selection using SVC
<img src="https://github.com/user-attachments/assets/658ec375-8bdf-4078-82c6-600e6b40799e" width="300" height="400">

## Top 5 Features 
### Sum Freq, Var Freq, Max Freq, Kurtosis Freq, Peak Freq

Accuracy - RFC: 74.66 %<br/>
Accuracy - SVC: 78.00 %<br/>

## Dimension Reduction

Accuracy - RFC: 78.20 % <br/>
Accuracy - SVC: 82.77 %
