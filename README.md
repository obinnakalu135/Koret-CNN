Koret - Solar Eclipse Image Classification

This project implements a deep learning model to classify images of solar eclipse phenomena. The model uses transfer learning with a pre-trained InceptionV3 model and incorporates data augmentation techniques to improve generalization.

Key Features:

Data Loading and Preprocessing:
Loads images from a directory structure with subfolders representing classes.
Preprocesses images by resizing and normalizing them.
Data Augmentation:
Applies random flips, rotations, brightness adjustments, and contrast adjustments to training images for improved robustness.
Class Imbalance Handling:
Analyzes class distribution and identifies imbalanced classes.
Oversamples minority classes using RandomOverSampler from imbalanced-learn library.
Model Architecture:
Leverages pre-trained InceptionV3 model for feature extraction.
Freezes initial layers of the pre-trained model for fine-tuning.
Adds custom layers for classification, including Dense layers with ReLU activation and Dropout for regularization.
Training and Evaluation:
Compiles the model with Adam optimizer, categorical crossentropy loss, and accuracy metric.
Trains the model using the oversampled training dataset.
Monitors validation accuracy and employs learning rate reduction and early stopping callbacks.
Getting Started:

Install required libraries: tensorflow, keras, numpy, pandas, imbalanced-learn, etc. (see code for full list).
Download the solar eclipse image dataset and organize it into subfolders representing classes.
Set the data_dir variable in the code to point to your data directory.
Run the script.
