# DEEP-LEARNING-PROJECT-CIE-1-
PROJECT IS ABOUT TO RECOGNIZE THE TRAFFIC SIGNAL USING RGB DATA SET 

Traffic Sign Recognition using PyTorch 🚗🚦

An end-to-end Computer Vision project that trains a custom Convolutional Neural Network (CNN) using PyTorch  to detect and classify traffic signs into 43 distinct categories. Designed for applications in Autonomous Driving and Advanced Driver Assistance Systems (ADAS).

 📌 Project Overview

Automated traffic sign recognition is a critical component for perception modules in autonomous vehicles. This repository contains a deep learning pipeline built from scratch to perform multi-class image classification on road signs under varying environmental conditions (lighting, weather, shadows, and physical wear).

🏗️ Model Architecture ( TrafficSignCNN )

The project utilizes a custom 2D CNN architecture structured into feature extraction and classification blocks:

Feature Extractor :
 2D Convolutional Layers (Conv2d) for spatial feature extraction.

Batch Normalization ( BatchNorm2d ) for faster convergence and training stability.

ReLU Activation functions for non-linearity.

Max Pooling (`MaxPool2d`) for spatial downsampling.

Dropout (`p=0.25`) for early regularization.

Classifier :

Flattening layer converting spatial feature maps into a 1D vector.

Fully Connected / Linear layers ( nn.Linear ).

High Dropout ( p=0.5 ) to prevent overfitting.

43 output logits corresponding to traffic sign categories.

📊 Dataset

Dataset :  German Traffic Sign Recognition Benchmark (GTSRB)

Classes :  43 categories (Speed limits, yield, stop, warnings, etc.)

Input Resolution :  $32 \times 32 \times 3$ (RGB)

Preprocessing :  Pixel normalization ($[0, 255] \rightarrow [0.0, 1.0]$) and spatial resizing.
 
🛠️ Tech Stack & Tools

Language :  Python
Framework :  PyTorch
Data Processing : NumPy, OpenCV / torchvision
Visualization :  Matplotlib

🚀 Key Features

 Custom CNN architecture built from scratch in PyTorch.
 Built-in batch normalization and dropout layers to mitigate overfitting.
 Multi-class classification optimization using Categorical Cross-Entropy Loss and the Adam optimizer.
 Modular and easily adaptable code structure for further fine-tuning on real-world datasets.
