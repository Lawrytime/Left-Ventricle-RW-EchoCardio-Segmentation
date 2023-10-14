# Left Ventricle Regional Wall Segmentation on Apical-4-Chamber (A4C) View 2D Echocardiography Recordings

## Overview

**This repository contains the code and resources for a deep learning project aimed at automating the segmentation of the left ventricle's regional wall in 2D apical-4-chamber (A4C) echocardiography recordings. Accurate segmentation of the left ventricle is crucial in the field of cardiology for assessing cardiac health and function.**


**The project leverages the UNet architecture, a popular choice for medical image segmentation tasks. It explores the use of two different loss functions, Dice Loss and Focal Tversky Loss, for optimizing the model's performance. Additionally, the project includes visualization techniques, such as saliency maps and learned filter visualization, to gain insights into the model's internal representations and attention patterns.**


## Key Features

  - UNet-based deep learning model for left ventricle regional wall segmentation.

    ![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/my_UNet.png)

    
  - Implementation and comparison of two loss functions: Dice Loss and Focal Tversky Loss.
  - Visualization of saliency maps to understand model attention.
  - Visualization of learned filters in convolutional layers for feature analysis.


## Dataset

The project utilizes the HMC-QU Dataset of 2D A4C echocardiography recordings available at [HMC-QU Dataset](https://www.kaggle.com/datasets/aysendegerli/hmcqu-dataset?select=LV+Ground-truth+Segmentation+Masks). It is essential to ensure that all patient details in the dataset have been anonymized to protect privacy and comply with ethical guidelines.

## Getting Started

To replicate or build upon this project, follow these steps:

Clone this repository to your local machine.
Set up your Python environment with the required dependencies (listed in requirements.txt).
Explore the Jupyter notebooks provided in the notebooks directory for model training and evaluation.
Customize hyperparameters, loss functions, and visualization as needed for your specific task.


## Results

The model achieved high precision, recall, accuracy, IoU, and F1 scores on the test dataset, indicating robust segmentation performance.
Saliency maps and learned filter visualization provide insights into model behavior and feature detection.

## License
This project is licensed under the MIT License.
