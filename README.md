# Medical Scan report Classification

## Description: 
The Medical Scan report classification is a jupyter notebook written in Python. The notebook contains the steps to train and infer a custom-designed CNN architecture to classify 6 class types of medical reports. 

## Key Features:
1. Custom CNN architecture to classify ['HeadCT', 'Hand', 'CXR', 'AbdomenCT', 'ChestCT', 'BreastMRI'].
2. The notebook helps beginners understand how to train a custom model to classify images.
3. The notebook also discusses image data augmentation and its importance in classifier training.


## Table of Contents
- [Usage](#usage)
- [Results](#results)

## Usage
1) Clone the MedicalScanReport_Classification repository:
   * `git clone https://github.com/NigamKatta/MedicalScanReport_Classification.git`
2) Download the MedNIST_dataset from the [link](https://drive.google.com/file/d/1HeQ-k-FOCESqOzFz7QNxRBtksIB2ONYG/view?usp=sharing).
3) Extract the dataset: ['HeadCT', 'Hand', 'CXR', 'AbdomenCT', 'ChestCT', 'BreastMRI'], type = Images
4) Run the cells in the notebook. The book is cuda supported.

## Results
**Test Accuracy:** 0.9518
**Precision:** 0.9513
**Recall:** 0.9508
**F1 Score:** 0.9505
**Confusion matrix:**
|            | Class 1 | Class 2 | Class 3 | Class 4 | Class 5 | Class 6 |
|------------|---------|---------|---------|---------|---------|---------|
| Predicted 1| 155     | 5       | 0       | 0       | 0       | 11      |
| Predicted 2| 6       | 201     | 6       | 0       | 1       | 1       |
| Predicted 3| 1       | 5       | 211     | 0       | 1       | 0       |
| Predicted 4| 0       | 0       | 0       | 186     | 4       | 0       |
| Predicted 5| 0       | 0       | 2       | 16      | 163     | 0       |
| Predicted 6| 0       | 0       | 0       | 0       | 0       | 225   

#### Visualization Demo
![a](![Screenshot from 2024-03-20 01-13-19](https://github.com/NigamKatta/MedicalScanReport_Classification/assets/115204043/c64aa34c-c6e7-4185-83d0-410109f19df3))
The title shows the model predictions from the classifier, and the x-label represents the ground truth.
