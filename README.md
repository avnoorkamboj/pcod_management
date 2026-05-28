# PCOS Detection using Ultrasound Image Analysis and Machine Learning

Overview

This project focuses on detecting Polycystic Ovary Syndrome (PCOS) using ultrasound image analysis and machine learning techniques.

The notebook processes ovarian ultrasound images, extracts medically relevant features such as cyst count and texture characteristics, and uses a machine learning classifier to predict the presence of PCOS.

The project demonstrates how computer vision and machine learning can assist in faster and more consistent medical image analysis.

# Problem Statement

PCOS is a hormonal disorder commonly diagnosed by observing multiple ovarian cysts in ultrasound scans. Manual diagnosis can:

Take significant time
Be subjective
Depend on radiologist expertise

This project automates part of the process by:

Detecting cyst-like regions
Extracting texture and shape features
Training a classifier for PCOS prediction

# Dataset

The project uses ovarian ultrasound images categorized into:

Infected / PCOS
Not Infected / Normal

The images are used to extract features related to:

Cyst count
Texture patterns
Area distribution
Image contrast

# Workflow
Ultrasound Images
        ↓
Image Preprocessing
        ↓
Contrast Enhancement (CLAHE)
        ↓
Thresholding & Contour Detection
        ↓
Feature Extraction
        ↓
Machine Learning Classification
        ↓
PCOS Prediction

# Features Extracted

The notebook extracts several important features from ultrasound images:

Image Features
Cyst count
Area ratio
Texture contrast
Homogeneity
Energy
Correlation
Image Processing Techniques
Grayscale conversion
CLAHE contrast enhancement
Binary thresholding
Contour detection
Noise filtering

# Machine Learning Model

The project uses:

Random Forest Classifier

Used for:

Feature-based classification
Pattern recognition
PCOS prediction

Why Random Forest?

Handles nonlinear patterns well
Robust to noise
Good performance on structured features

# Technologies Used
Python
OpenCV
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
Scikit-image

# Project Structure
.
├── ML_Project.ipynb
├── README.md
├── data/
│   ├── train/
│   │   ├── infected/
│   │   └── notinfected/
│   └── test/
├── models/
└── outputs/

# Installation
1. Clone the Repository
git clone https://github.com/your-username/pcos-ultrasound-detection.git
cd pcos-ultrasound-detection
2. Install Dependencies
pip install -r requirements.txt

Or manually install:

pip install opencv-python numpy pandas matplotlib seaborn scikit-learn scikit-image

# Usage

Run the Notebook
jupyter notebook ML_Project.ipynb

Run the notebook cells sequentially to:

Load ultrasound images
Preprocess images
Extract features
Train the Random Forest model
Evaluate prediction results

# Image Preprocessing

The project applies several preprocessing techniques:

CLAHE (Contrast Limited Adaptive Histogram Equalization)

Used to:

Enhance ultrasound contrast
Improve cyst visibility
Reduce uneven illumination
Thresholding

Used to:

Convert images into binary format
Separate cyst regions from background
Contour Detection

Used to:

Detect cyst boundaries
Measure cyst-related features

# Data Visualization

The notebook includes:

Boxplots
Scatter plots
Feature distribution analysis
Correlation visualization

These help understand how extracted features differ between normal and PCOS images.

# Evaluation Metrics

The model evaluation may include:

Accuracy
Precision
Recall
F1-Score
Confusion Matrix
Classification Report

# Results

The system is designed to:

Detect cyst-like regions automatically
Extract meaningful texture features
Assist in early PCOS prediction
Reduce manual diagnostic effort

You can add:

Final accuracy scores
Confusion matrices
Sample output images
Performance graphs

# Future Improvements

Potential enhancements:

Deep learning using CNNs
Real-time ultrasound analysis
Segmentation-based cyst detection
Deployment as a web application
Multi-class ovarian condition classification

# References
PCOS Ultrasound Imaging Research Papers
OpenCV Documentation
Scikit-learn Documentation
Medical Image Processing Literature

