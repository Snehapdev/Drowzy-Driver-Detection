# Project Report: Image Classification with Deep Learning

## Introduction
This project aims to develop a deep learning model for image classification using PyTorch. The dataset used consists of images of eyes and mouths, categorized into two classes: "yawn" and "no_yawn".

## Dataset Description
- **Source:** The dataset was obtained from Kaggle, containing images of eyes and face of people in various states(yawn, not-yawn)
- **Preprocessing:** Images were resized to 256x256 pixels and normalized.
- **Class Distribution:** Approximately equal distribution between "yawn" and "no_yawn" classes.

## Model Architecture
- **Custom CNN:** Three convolutional layers followed by max-pooling and global average pooling layers, and two fully connected layers.
- **Transfer Learning:** Pre-trained ResNet18 with the final fully connected layer replaced.

## Training Process
- **Data Augmentation:** Random horizontal flipping and rotation.
- **Loss Function:** Cross-entropy.
- **Optimizer:** Adam with lr=0.001.
- **Training:** 30 epochs with mini-batch SGD for Custom CNN, 10 epochs with mini-batch SGD for Transfer learning model

## Results and Discussion
- **Custom CNN:** Validation accuracy: 71.12%, Test accuracy: 74.60%.
- **Transfer Learning (ResNet18):** Validation accuracy: 91.89%, Test accuracy: 88.68%.
- **Interpretation:** Used class activation maps for insights.

## Conclusion
The models demonstrated promising performance, with ResNet18 outperforming the custom CNN architecture.

## How to Run the Project
1. Download the kaggle.json file.
2. Load the kaggle.json file before executing the notebook.

