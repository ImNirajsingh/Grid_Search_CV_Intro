<<<<<<< HEAD
# Iris Dataset Classification & Hyperparameter Tuning

Welcome to this project! This repository contains a Jupyter Notebook dedicated to classifying flower species from the classic Iris dataset using machine learning[cite: 1]. The primary focus of this project is not just on building predictive models, but on demonstrating how to systematically optimize them using advanced hyperparameter tuning techniques[cite: 1]. 

## 📖 About the Project

This project walks through a complete machine learning workflow. It starts with basic data loading and split techniques, establishes baseline classification models, and then dives deep into tuning those models to squeeze out the best possible accuracy[cite: 1]. 

Specifically, it compares standard hyperparameter tuning using a comprehensive **Grid Search** against a more efficient **Randomized Search**[cite: 1].

## 🛠️ Built With

This project relies on the core Python data science stack[cite: 1]:
*   **Data Manipulation:** `numpy`, `pandas`[cite: 1]
*   **Data Visualization:** `seaborn`, `matplotlib.pyplot`[cite: 1]
*   **Machine Learning:** `scikit-learn` (`KNeighborsClassifier`, `SVC`, `train_test_split`, `GridSearchCV`, `RandomizedSearchCV`)[cite: 1]

## 🧠 What's Inside the Notebook

Here is a breakdown of the workflow you will find inside the notebook `GridSearchCV.ipynb`[cite: 1]:

1.  **Data Loading & Preparation:** 
    *   Loads the 'iris' dataset directly through Seaborn[cite: 1].
    *   Isolates the target variable (`species`, consisting of 'setosa', 'versicolor', and 'virginica') from the descriptive features[cite: 1].
    *   Splits the data into training and testing sets using an 80/20 split (`test_size=0.20`) with a fixed random state for reproducibility[cite: 1].

2.  **Baseline Modeling:**
    *   Initializes and trains a **K-Nearest Neighbors (KNN)** classifier starting with 13 neighbors[cite: 1].
    *   Initializes and trains a **Support Vector Classifier (SVC)** using automatic gamma scaling[cite: 1].

3.  **Hyperparameter Optimization (Grid Search):**
    *   **SVM Grid Search:** Applies `GridSearchCV` with 5-fold cross-validation to exhaustively test different combinations of the `C` parameter (1, 10, 20, 30) and `kernel` types ('rbf', 'linear')[cite: 1].

    *   **KNN Grid Search:** Applies `GridSearchCV` to test various neighbor counts (5, 7, 10, 12) alongside different underlying algorithms ('auto', 'ball_tree', 'kd_tree', 'brute')[cite: 1].
    *   Converts the cross-validation results into easy-to-read Pandas DataFrames to compare the mean test scores[cite: 1].

4.  **Hyperparameter Optimization (Randomized Search):**
    *   Implements `RandomizedSearchCV` on the SVM model as a faster alternative to Grid Search[cite: 1].
    *   Samples 4 iterations (`n_iter=4`) from the predefined parameter grid to find an optimal model efficiently[cite: 1].

## 🚀 Getting Started

To run this notebook locally, ensure you have Python installed along with the required libraries. 

1. Clone this repository to your local machine.
2. Install the required dependencies:
   ```bash
   pip install numpy pandas seaborn matplotlib scikit-learn



Niraj Singh
=======
# Grid_Search_CV_Intro
A beginner-friendly introduction to hyperparameter tuning and model optimization using GridSearchCV in scikit-learn.
>>>>>>> 9019629af87ac3c9e8dad37b57a1b4950428048d
