# Medical Scan report Classification

## Description: 
The Complex YOLO ROS 3D Object Detection project is an integration of the [Complex YOLOv4](https://github.com/maudzung/Complex-YOLOv4-Pytorch) package into the ROS (Robot Operating System) platform, aimed at enhancing real-time perception capabilities for robotics applications. Using 3D object detection techniques based on Lidar data, the project enables robots and autonomous systems to accurately detect and localize objects in a 3D environment, crucial for safe navigation, obstacle avoidance, and intelligent decision-making.
The Medical Scan report classification is a jupyter notebook which is written in Python. The notebook contains the steps to train and infer a Custom Designed CNN architecture in order to classify 6 class types of medical reports. 

## Key Features:
1. Custom CNN architecture to classify ['HeadCT', 'Hand', 'CXR', 'AbdomenCT', 'ChestCT', 'BreastMRI'].
2. The notebook helps begineers understand how to train a custom model in order to classify images.
3. The notebook also talks about image data augumentation and it's importance in training a classifier.


## Table of Contents
- [Usage](#usage)
- [Results](#results)


## Usage
1) Clone the MedicalScanReport_Classification repository:
   * `git clone https://github.com/NigamKatta/MedicalScanReport_Classification.git`
2) Download the MedNIST_dataset from the [link](https://drive.google.com/file/d/1HeQ-k-FOCESqOzFz7QNxRBtksIB2ONYG/view?usp=sharing).
3) Extract the dataset: ['HeadCT', 'Hand', 'CXR', 'AbdomenCT', 'ChestCT', 'BreastMRI'] , type = Images
4) Run the cells in the notebook. The book is cuda supported.

## Results
Test Accuracy: 0.9518
Precision: 0.9513, Recall: 0.9508, F1 Score: 0.9505
Confusion matrix:
[[155   5   0   0   0  11]
 [  6 201   6   0   1   1]
 [  1   5 211   0   1   0]
 [  0   0   0 186   4   0]
 [  0   0   2  16 163   0]
 [  0   0   0   0   0 225]]

#### Visualization Demo
![a](![Screenshot from 2024-03-20 01-13-19](https://github.com/NigamKatta/MedicalScanReport_Classification/assets/115204043/c64aa34c-c6e7-4185-83d0-410109f19df3))
The top tile is the predictions from the classifier, the True represented the ground truth.
