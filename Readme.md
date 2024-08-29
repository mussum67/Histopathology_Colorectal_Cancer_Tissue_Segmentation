# Colorectal Cancer Detection Using Histopathology Images

Colorectal Cancer is one of the leading causes of death, and early detection is essential to prevent premature mortality. This project utilizes various techniques to analyze histopathology images for the early detection of Colorectal Cancer.

## Project Overview

The project is divided into three main approaches:

1. **Advanced Image Processing**:
   - Implemented advanced image processing algorithms such as morphology, unwanted object removal, and watershed segmentation.
   - These techniques were used to segment images, detect tumors and polyps, and differentiate between normal and abnormal cases.

2. **Feature Extraction and Classification**:
   - Feature extraction was performed using image descriptor techniques like:
     - Local Binary Pattern (LBP)
     - Gabor Filter
     - Histogram of Oriented Gradients (HOG)
   - Machine learning algorithms were then employed to classify the images into different classes based on the extracted features.

3. **Deep Learning Approach**:
   - Developed a U-Net architecture for the segmentation of histopathology images.
   - To capture the complex features of colorectal cancer tissues, the model architecture was enhanced with:
     - Integration of various encoding and decoding blocks
     - Bottleneck layer
     - Skip connections
   - The architecture allows for customizable depths and the number of filters (Batch size, learning rate, and number of epochs are configurable).

## Implementation Details

- The project implementation was carried out using the PyTorch framework, with Weights & Biases utilized for visualizing the learning curves.
- **GPU Memory Management**: The code includes commands to ensure efficient resource use during training.
- **Loss Function**: Dice Loss was employed as the loss function for both training and validation.
- **Performance Evaluation**: The model’s performance was evaluated using the learning curves of training and validation losses.

## Inference

- The Inference Notebook provides segmented output images alongside the original inputs, allowing for observation of the model’s performance.

## Dataset

- [Link to the dataset](https://drive.google.com/drive/folders/1UB86gL0XwiShc8n2ONwA_YshQ2xQDPXV?usp=drive_link)

