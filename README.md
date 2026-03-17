# Forest Cover Type Prediction using Machine Learning

## Overview

This project focuses on predicting forest cover types using supervised machine learning techniques. It also serves as a comparative framework for evaluating the performance of multiple classification algorithms on the same dataset.

The system uses cartographic and environmental features to classify forest areas into different categories.

---

## Objective

* To build a machine learning model for predicting forest cover types
* To compare the performance of different classification algorithms
* To analyze how different models behave on structured environmental data

---

## Dataset Description

* Source: US Forest Service (USFS) Region 2 Resource Information System
* Each record represents a 30 × 30 meter forest cell
* Training dataset size: 15,120 samples
* Test dataset contains only feature values

### Target Variable

The dataset contains 7 forest cover types:

1. Spruce/Fir
2. Lodgepole Pine
3. Ponderosa Pine
4. Cottonwood/Willow
5. Aspen
6. Douglas-fir
7. Krummholz

### Features

The dataset includes both numerical and categorical variables such as:

* Elevation, Aspect, Slope
* Distance to hydrology, roadways, and fire points
* Hillshade indices (9am, Noon, 3pm)
* Wilderness area indicators (4 binary columns)
* Soil type indicators (40 binary columns)

---

## Dataset Note

The dataset is not included in this repository. It can be obtained from public sources such as Kaggle or other platforms .

---

## Data Preprocessing

* Handling missing values
* Feature scaling for numerical variables
* One-hot encoding for categorical features
* Splitting data into training, validation, and test sets

---

## Models Implemented

The following machine learning models are implemented and evaluated:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* XGBoost Classifier
* CatBoost Classifier
* K-Nearest Neighbors (KNN)
* Extra Trees Classifier
* Neural Network (TensorFlow/Keras)

---

## Use as a Testing Framework

In addition to prediction, this project can be used as a base framework to:

* Test and compare different machine learning algorithms
* Evaluate model performance on the same dataset
* Experiment with feature engineering and preprocessing techniques
* Perform hyperparameter tuning
* Analyze accuracy differences across models

---

## Neural Network Architecture

* Two hidden layers with ReLU activation
* Output layer with Softmax activation (7 classes)
* Optimizer: Adam
* Loss function: Categorical Crossentropy

---

## Results and Performance

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 66.6%    |
| Decision Tree       | 94.9%    |
| Random Forest       | 95.0%    |
| XGBoost             | 87.20%   |
| CatBoost            | 87.50%   |
| KNN                 | 80.36%   |
| Neural Network      | 89.52%   |
| Extra Trees         | 86.84%   |

Random Forest, Decision Tree, and Neural Network models achieved the highest performance.

---

## Project Structure

├── forest_cover_type_prediction.py
├── Forest_Cover_Type_Prediction.ipynb
├── B.Tech last yr project report.pdf
└── README.md

---

## Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* TensorFlow / Keras
* XGBoost, CatBoost
* Matplotlib, Seaborn
* Google Colab

---

## How to Run

1. Open the notebook or Python file in Google Colab or a local environment

2. Install required libraries if needed:
   pip install pandas numpy scikit-learn tensorflow xgboost catboost matplotlib seaborn

3. Load the dataset and execute the code

---

## Conclusion

The project demonstrates that ensemble learning methods such as Random Forest and Decision Tree provide strong performance for this classification problem. Neural networks also achieve competitive results.

---

## Future Work

* Hyperparameter tuning
* Model optimization
* Deployment using web frameworks
* Integration with real-world data sources

---

## Author

Sayan Barik
B.Tech, Computer Science and Engineering
Maulana Abul Kalam Azad University of Technology, West Bengal
