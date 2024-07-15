# Pixelated Image Detection and Correction

## Project Overview

This project aims to develop a system for detecting and restoring pixelated images. By leveraging a convolutional autoencoder and a classifier, the model is designed to handle high-resolution images efficiently, ensuring high accuracy and performance in real-time applications.

## Problem Statement

Detecting pixelation in images and restoring them to their original quality without compromising details or introducing artifacts.

## Solution

1. **Pixelation Detection**: 
   - Utilizes a lightweight convolutional autoencoder to encode and decode image features.
   - Classifies images as pixelated or non-pixelated using a dense layer for high FPS and accuracy.
   
2. **Image Restoration**:
   - Designs an efficient convolutional autoencoder to restore pixelated images, maintaining high quality and detail.

## Features

- Real-time pixelation detection at 60 FPS.
- High accuracy and F1 score with low false positives.
- Quality restoration of pixelated images without affecting non-pixelated images.
- Scalable and versatile model for various devices and screen sizes.

## Architecture

1. **Preprocessing**: Image resizing and normalization.
2. **Pixelation Detection**: Feature extraction and classification.
3. **Image Restoration**: Image restoration using a generator model.
4. **Evaluation Metrics**: Calculation and evaluation of quality metrics.
5. **Logging and Monitoring**: Logging requests and monitoring model performance.
6. **Error Handling**: Handling and logging errors, returning error messages.

## Technologies Used

- **TensorFlow**: Model building and deployment.
- **Keras**: Simplifies model creation and training.
- **Convolutional Neural Networks (CNN)**: Efficient spatial feature extraction.
- **Autoencoder**: Captures and reconstructs image details.
- **ImageDataGenerator**: Enhances generalization with efficient image splitting and resizing.
- **Adam Optimizer**: For efficient learning.
- **OpenCV**: Image preprocessing and manipulation.
- **Matplotlib**: For visualization.

## Team Members

- **R Rufus Clieve Roy**: Project Lead and Software Engineer - [Email](mailto:sec22mu023@sairamtap.edu.in)
- **N Gopika**: Data Scientist and Research Analyst - [Email](mailto:sec22ec149@sairamtap.edu.in)

## Dataset

The dataset used for training is original and pixelated images, which can be found [here](https://drive.google.com/drive/folders/1A4ukgyqmHCeZjeZJIMFBo8d7YTeznE5w?usp=sharing).

## Model Experiments

| Model       | Accuracy | F1 Score | Size  | 
|-------------|----------|----------|-------|
| Autoencoder | 78%      | 0.70     | 2MB   |
| MobileNet   | 60%      | 0.58     | 29MB  |
| SVM         | 68%      | 0.51     | 16MB  |
| AlexNet     | 50%      | 0.48     | 23MB  |
| ResNet      | 50%      | 0.43     | 28MB  |
| InceptionV3 | 78%      | 0.49     | 9MB   |

### Rejected Models

Some models were rejected based on their performance metrics and efficiency:

- **MobileNet**: Rejected due to relatively low accuracy (60%) and F1 score (0.58) despite having a larger model size (29MB).
- **AlexNet**: Rejected due to poor accuracy (50%) and F1 score (0.48), indicating it was not effective in differentiating between pixelated and non-pixelated images.
- **ResNet**: Rejected for similar reasons to AlexNet, with an accuracy and F1 score of 50% and 0.43, respectively, making it unsuitable for our needs.
- **InceptionV3**: Despite having a better accuracy (78%) than some other models, its F1 score (0.49) was not satisfactory, leading to its rejection.

## Conclusion

- **Objective**: Developed a system to detect and restore pixelated images.
- **Approach**: Trained an autoencoder for image reconstruction and built a classifier for pixelated image detection.
- **Model Performance**: Achieved 72% accuracy and F1 score of 0.70.
- **Model Efficiency**: Lightweight models suitable for resource-constrained environments.
- **Visual Results**: Effective restoration of original quality of pixelated images and clear separation in predictions.
- **Future Work**: Implement more sophisticated network architectures and optimize models for real-time deployment.

## Report

For a detailed report on the reject projects, please refer to the [rejected_model report](https://drive.google.com/drive/folders/1xo0KZliQBSj07DAy8uPIl0-87xC7nKlu?usp=sharing).


For a detailed report on the working project, please refer the [Final_project](https://drive.google.com/drive/folders/1AhL5n2vOYQA1O2_6o8jvPC0WjXC5AXJP?usp=sharing)
