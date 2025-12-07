<img width="1536" height="1024" alt="ChatGPT Image Dec 7, 2025, 12_25_06 PM" src="https://github.com/user-attachments/assets/c0460a26-6613-4cb3-b703-4e1d89f614c8" />



# UTKFace Multi-Output Age, Gender & Race Prediction

A deep learning project using TensorFlow Keras Functional API to build a multi-output CNN model that predicts:

1. Age (Regression)
2. Gender (Binary Classification)
3. Race (Multi-Class Classification)

# Project Overview

This project uses the UTKFace Dataset, a large-scale face dataset with labels for age, gender, and ethnicity.
The goal is to train a single neural network that outputs all three predictions simultaneously.

### What this model does:

Extracts facial features with CNN layers

1. Uses Global Average Pooling for efficient feature aggregation
2. Splits into three separate dense heads for multi-task learning
3. Trains all outputs jointly with optimized loss weighting

# Dataset

Dataset Used: UTKFace (Faces with Age, Gender & Race labels):
URL: https://www.kaggle.com/datasets/jangedoo/UTKFace-new

# Model Architecture (Functional API)

The model uses:

1. Input Layer
2. Conv2D + MaxPooling2D Blocks
3. Global Average Pooling

### Three Output Heads:

1. Dense(1) → Age
2. Dense(1, sigmoid) → Gender
3. Dense(num_classes, softmax) → Race

# Summary:

1. Multi-output model
2. Shared CNN backbone
3. Efficient feature learning
4. Handles different tasks in one forward pass

# Project Structure

 Multi-Output-UTKFace-Model.
 
 ┣ dataset
 
 ┣ Functional_model(Multi_output_code).ipynb
 
 ┣ README.md
 
 ┗ requirements.txt
