# Left Ventricle Regional Wall Segmentation on Apical-4-Chamber (A4C) View 2D Echocardiography Recordings

##  

![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/LV_Segmentation_Intro.jpg)

## 

## Content
- [Project Overview](#overview)
- [Key Features](#key)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training and Evaluation](#training-and-evaluation)
- [Results](#results)
- [Saliency Maps](#saliency-maps)

##  

## Overview

This repository contains the code and resources for a deep learning project aimed at automating the segmentation of the left ventricle's regional wall in 2D apical-4-chamber (A4C) echocardiography recordings. Accurate segmentation of the left ventricle is crucial in the field of cardiology for assessing cardiac health and function.


The project leverages the UNet architecture, a popular choice for medical image segmentation tasks. It explores the use of two different loss functions, Dice Loss and Focal Tversky Loss, for optimizing the model's performance. Additionally, the project includes visualization techniques, such as saliency maps and learned filter visualization, to gain insights into the model's internal representations and attention patterns.

##  

## Key Features

  - UNet-based deep learning model for left ventricle regional wall segmentation.    
  - Implementation and comparison of two loss functions: Dice Loss and Focal Tversky Loss.
  - Visualization of saliency maps to understand model attention.
  - Visualization of learned filters in convolutional layers for feature analysis.


## Dataset

The project utilizes the HMC-QU Dataset of 2D A4C echocardiography recordings available at [HMC-QU Dataset](https://www.kaggle.com/datasets/aysendegerli/hmcqu-dataset?select=LV+Ground-truth+Segmentation+Masks). It is essential to ensure that all patient details in the dataset have been anonymized to protect privacy and comply with ethical guidelines.

##  

## Model Architecture

This project employed a convolutional neural network (CNN) based on the UNet architecture. UNet is known for its effectiveness in image segmentation tasks and has been customized to suit the specific requirements as this task is semantic segmentation on video data.

The architecture comprises several key components:

  - Downsample Path: This path includes convolutional layers with ReLU activation functions for feature extraction and down-sampling via max-pooling operations.

  - Bottleneck: A bottleneck layer that further extracts and consolidates features.

  - Upsample Path: The upsample path employs transposed convolutional layers for feature expansion and up-sampling.
   ![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/my_UNet.png)

  - Loss Function: Two loss functions were evaluated: Dice Loss and Focal Tversky Loss. Hyperparameter tuning was conducted to select the best-performing loss function.
    
  ## Dice Loss

  ![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/Dice_Loss.png)
  
  ![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/Dice_L.png)


  ## Focal Tversky Loss
  
  ![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/Focal_Tversky_Loss.png)
  
  ![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/Focal_Tversky_L.png)


##  

## Training and Evaluation

The model was trained using a combination of training and validation datasets. During training, several evaluation metrics were monitored.

    Dice coefficient, IoU, Accuracy
    Precision, Recall, F1 score

##  

## Results

The model achieved high precision, recall, accuracy, IoU, and F1 scores on the test dataset, indicating robust segmentation performance.
Saliency maps and learned filter visualization provide insights into model behavior and feature detection.

![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/Segmentations/Segmentation%20with%20Dice%20Loss.png)

##  

![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/Segmentations/Segmentation%20with%20Focal%20Tversky%20Loss.png)

##  

## Saliency Maps

In addition to segmentation, saliency maps were generated to visualize the model's attention patterns on the regional walls of the left ventricle. Furthermore, learned filters in convolutional layers were visualized to understand the model's feature detection capabilities.
![](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/assets/Saliency%20Maps.png)

##  

## License
This project is licensed under the [MIT License](https://github.com/Lawrytime/Left-Ventricle-RW-EchoCardio-Segmentation/blob/main/LICENSE).
