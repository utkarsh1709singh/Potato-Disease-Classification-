
#Plant Disease Classification using Machine Learning#

This repository contains Python code for a plant disease classification project using machine learning. The project uses a dataset from PlantVillage, and it demonstrates the process of loading, preprocessing, and classifying plant disease images.

Getting Started

Prerequisites
Make sure you have the following libraries installed:
bash (pip install pandas matplotlib opencv-python keras tensorflow scikit-learn)

Dataset
Download the PlantVillage dataset from PlantVillage and set the dataset_path variable in the script to the location of your dataset.

Code Overview

Data Preparation

Import necessary libraries.

Set the path to the dataset.

Extract a list of image files and their corresponding class labels.

Create a DataFrame to store information about the images.

Image Preprocessing

Define a function to preprocess individual images.
Apply the preprocessing function to all images in the dataset.

Data Splitting

Split the data into training and testing sets (80% training, 20% testing).

Feature Extraction using VGG16

Load the pre-trained VGG16 model without the top (fully connected) layers.
Define a function to extract features using VGG16.

Apply the feature extraction function to the training and testing sets.

Model Training and Evaluation

Train logistic regression, k-nearest neighbors, naïve Bayes, and support vector machine (SVM) models.
Evaluate the models using accuracy and classification reports.

Image Prediction

Define a function to preprocess a single image and display the original and preprocessed images.
Extract features from the preprocessed image.
Make predictions using the trained models and display the results.

Usage
Ensure that the dataset is downloaded and the dataset_path variable is set correctly.
Run the script in a Python environment.
Example Usage for Single Image Prediction

To predict the class of a new image, follow these steps:

Set the new_image_path variable to the path of the new image.
Run the script.
The original and preprocessed images will be displayed, along with predictions from the logistic regression, k-nearest neighbors, naïve Bayes, and SVM models.

Feel free to experiment with different images and adapt the code for your specific use case.

Note: Make sure to adhere to the license terms of the PlantVillage dataset when using the images for your project.

License
This project is licensed under the MIT License - see the LICENSE file for details.
