# FACE IT : Personalised Skincare and Makeup Recommendation System.
## Overview
This project presents an AI-powered Personalized Skincare and Makeup Recommendation System that analyzes a user's facial image (selfie) using Computer Vision and Deep Learning techniques to recommend suitable skincare and makeup products.

The system extracts key skin metrics such as:
Skin Type (Oily, Dry, Normal)
Skin Tone (Fitzpatrick Scale)
Acne Severity (Low, Moderate, Severe)

Based on these metrics, the system recommends skincare products that best match the user's skin characteristics using a content-based recommendation system with cosine similarity.

The application is built using React for the frontend and Flask for the backend, enabling users to upload images and receive personalized product recommendations through a simple web interface.

## Problem Statement

Choosing the right skincare and makeup products is difficult because skin types and conditions vary from person to person. Most users rely on trial-and-error or generic recommendations that may not suit their skin.

This project aims to solve this problem by building an intelligent system that:

Analyzes skin conditions using computer vision

Identifies skin type, tone, and acne severity

Recommends suitable products automatically

The goal is to provide a virtual skincare advisor that makes skincare selection easier, faster, and more personalized.

## Features

- Skin type detection using EfficientNet B0

- Acne severity classification using CNN

- Skin tone detection using HSV and YCbCr color spaces

- Product recommendation using cosine similarity

- Web-based interface for image upload and results

- Personalized skincare suggestions

## Technologies Used
Frontend

- React.js

- HTML

- CSS

- JavaScript

 Backend

- Flask

- Python

Machine Learning & Image Processing

- TensorFlow / Keras

- OpenCV

- Scikit-learn

- NumPy

- EfficientNet B0

- CNN

## System Architecture

The system works in the following stages:

User uploads a selfie through the web interface

Image preprocessing is performed

CNN models extract skin metrics:

- Skin Type

- Acne Severity

- Skin tone is detected using color segmentation

- The extracted skin profile is converted into a feature vector

- Cosine similarity is used to match the user profile with product attributes

- Top matching products are recommended to the user

## Dataset

The project uses a combination of datasets:

Skin Type & Acne Dataset

Public datasets from Kaggle

Labeled images for:

- Oily skin

- Dry skin

- Normal skin

- Acne severity levels

- Skin Tone Dataset

- Processed facial images

- Skin regions extracted using HSV and YCbCr color spaces

Product Dataset

- Custom dataset created by scraping skincare products from Myntra

- Includes product attributes such as:

- Skin compatibility

- Target concerns

- Ingredients

## Model Performance
Model	Training Accuracy	Validation Accuracy
Skin Type Detection (EfficientNet B0)	~87%	~80%
Acne Severity Detection (CNN)	~68%	~68%
Sample Evaluation Metrics

Accuracy: 83.33%

F1 Score: 0.82

Recall: 0.83

Precision: 0.84

## Installation
1.  Clone the repository
cd faceit

2.  Create virtual environment
virtualenv my_env

3.  Activate environment

  Windows
  
  my_env\Scripts\activate
  
  Linux / Mac
  
  source my_env/bin/activate

4. Install dependencies
pip install -r requirements.txt
Running the Project

Start the Flask backend:

python app.py

Start the React frontend:

npm start

Open the application in the browser.

## Future Improvements

Detect additional skin concerns such as pigmentation and wrinkles

Improve acne classification accuracy with larger datasets

Integrate dermatologist knowledge bases

Add real-time camera analysis

Deploy as a mobile application

## Applications

Online skincare consultation

Beauty product recommendation systems

AI-powered dermatology assistants

E-commerce beauty platforms
