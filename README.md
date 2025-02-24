# Pneumonia-Image-Classification
This project aims to classify chest X-ray images as either Pneumonia or Non-Pneumonia using deep learning techniques. The implementation leverages Transfer Learning with InceptionV3 and explores both TensorFlow and Keras for model development.


Table of Contents
Overview
Why Transfer Learning?
Technologies Used
Model Implementation
Dataset
Results
Contributors
License


Overview
Pneumonia is a severe respiratory infection affecting millions worldwide, especially young children and the elderly. Traditional diagnosis through X-ray imaging requires expert interpretation, which can be time-consuming. This project introduces an automated deep learning model to assist in the early detection of pneumonia, reducing diagnostic time and improving accuracy.


Why Transfer Learning?
Since medical datasets are often limited due to privacy concerns, I utilized Transfer Learning with InceptionV3, a pre-trained model on ImageNet, to improve classification accuracy with minimal training data. This approach ensures: Faster training times, Improved feature extraction, Reduced risk of overfitting


Technologies Used
Deep Learning: TensorFlow, Keras
Data Processing: NumPy, Pandas
Visualization: Matplotlib
Hardware: GPU acceleration (NVIDIA CUDA recommended)


Model Implementation
Keras Approach
Pre-trained Model: InceptionV3 without top layers
Custom Layers: Global Average Pooling + Fully Connected Layers
Optimizer: Adam
Loss Function: Binary Cross-Entropy
Metrics: Accuracy
TensorFlow Approach
CNN Architecture: Convolutional & Pooling Layers
Optimizer: Adam
Data Augmentation: Rescaling, Rotation, Zooming
Training: 10 epochs


Dataset
Used a publicly available Chest X-ray dataset that contains:


Pneumonia X-rays
Non-Pneumonia X-rays (Healthy Lungs)


Results
Model	Accuracy
Keras (InceptionV3)	92.5%
TensorFlow CNN	88.3%

The Keras implementation achieved the highest accuracy, making it the preferred choice.

Contributors
Raza Mehdi
