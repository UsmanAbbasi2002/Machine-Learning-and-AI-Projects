# Iris Flower Dataset - Machine Learning Project

## Overview
This project analyzes the famous **Iris Flower Dataset** and applies various machine learning techniques to classify iris species based on their features. The dataset contains measurements of **sepal length, sepal width, petal length, and petal width** for three iris species: *Setosa, Versicolor, and Virginica*.

## Features of this Project
- **Exploratory Data Analysis (EDA)**: Univariate and multivariate analysis, visualizations, and outlier detection.
- **Data Preprocessing**: Handling missing values, normalizing features, and encoding categorical variables.
- **Model Training**: Implemented and tuned multiple models including:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - XGBoost
  - K-Nearest Neighbors (KNN) (Best Model - 100% Accuracy)
- **Hyperparameter Tuning**: Used **GridSearchCV** for optimizing model performance.
- **Model Saving**: The best-performing KNN model is saved as a `.pkl` file for future use.

## Results
After rigorous experimentation, **KNN with k=7, Euclidean distance, and uniform weights achieved 100% accuracy**, making it the best model.

## How to Use
1. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
2. Load the trained model:
   ```python
   import pickle

   with open('Iris_Flower_knn_model.pkl', 'rb') as model_file:
       knn_model = pickle.load(model_file)

   # Example prediction
   sample = [[5.1, 3.5, 1.4, 0.2]]
   prediction = knn_model.predict(sample)
   print("Predicted Iris Species:", prediction)
   ```

## Repository
Find the complete code and datasets on GitHub: [Iris Flower Dataset Project]([https://github.com/UsmanAbbasi2002/Iris_Flower_Dataset_Work/tree/main](https://github.com/UsmanAbbasi2002/Machine-Learning-and-AI-Projects/tree/main/Iris_Flower_Project)

## License
This project is open-source and available for educational purposes.
