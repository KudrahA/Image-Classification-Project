## Math3333---Image-Classification-Using-Machine-Learning-Models

## Image Classification with Machine Learning

This project is part of the final coursework for MATH 3333 at York University. It involves using various machine learning models to classify images from the Columbia Image dataset as either "outdoor-day" or "not outdoor-day" based on grid-based pixel intensity features.

## 📦 Dataset

- **Source**: Columbia Photographic Images and Photorealistic Computer Graphics Dataset  
- **Size**: 800 labeled images  
- **Labels**: 8 categories (e.g., indoor-light, outdoor-day, outdoor-night, etc.)
- **Target**: Binary classification — whether an image is `"outdoor-day"` or not

## 🔍 Project Overview

- **Baseline**: Logistic Regression (Instructor-provided code)
- **Feature Extraction**: 10×10 grid applied to each image, median intensity per R/G/B channel — 300 features per image
- **Models Used**:
  - Logistic Regression (baseline)
  - Random Forest
  - Linear Discriminant Analysis (LDA)
  - K-Nearest Neighbors (KNN)

## 📊 Evaluation Metrics

Models were evaluated on:
- Accuracy
- Sensitivity
- Specificity
- Misclassification Error
- ROC Curve and AUC

## 📁 Files Included

- `project_code.Rmd`: All preprocessing, model training, and evaluation code
- `photoMetaData.csv`: CSV with image names and category labels (not included in repo for copyright reasons)
- Image folder: `columbiaImages/` (not included in repo due to size — assumed to be in the working directory)

## 🚀 How to Run

1. Clone the repository
2. Open `project_code.Rmd` in RStudio
3. Update file paths to your local copies of the dataset and image folder
4. Knit or run the script chunk by chunk to generate model results

## 📈 Results Summary

| Model              | Accuracy | Sensitivity | Specificity | AUC    |
|-------------------|----------|-------------|-------------|--------|
| Random Forest      | 81.4%    | 63.4%       | 90.6%       | 0.859  |
| Logistic Regression| 74.1%    | 47.9%       | 88.9%       | 0.8294 |
| KNN (k=19)         | 76.6%    | 38.7%       | 96.0%       | 0.8334 |
| LDA                | 64.4%    | 52.1%       | 70.8%       | 0.6305 |

## ✍️ Author

Kudrah Asamu  
Final Project — MATH 3333 (2025)  
York University

