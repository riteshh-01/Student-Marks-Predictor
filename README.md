# 📚 Student Marks Predictor

This project is a machine learning notebook that predicts a student's expected marks based on their study hours. It applies a Linear Regression algorithm to model the linear relationship between an independent variable (study hours) and a single dependent variable (student marks).

# Click Here to have view of this project
Predicts a student's marks based on their study hours using Linear Regression.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/riteshh-01/Student-Marks-Predictor/blob/main/student_marks_prediction.ipynb)


## ✨ Features
* **Data Preprocessing**: Checks for missing values within the dataset and automatically fills empty data points with the column's mean value.
* **Data Visualization**: Generates a scatter plot (styled in pink) to visually analyze the relationship between "Study Hours" and "Student Marks".
* **Interactive Prediction**: Accepts custom user input for study hours (validating that the input is between 4 and 12 hours) and outputs the predicted academic score.

## 🛠️ Tech Stack & Libraries
This project is built using Python 3 (version 3.11.0) and relies on the following essential libraries:
* `pandas`: Used for importing the CSV dataset and separating independent/dependent variables.
* `numpy`: Imported for numerical array operations.
* `matplotlib.pyplot`: Utilized for generating the data scatter plot and grid visuals.
* `scikit-learn`: Provides the `train_test_split` function and the `LinearRegression` model.

## 📊 Dataset
The model requires a dataset named `student_info.csv` to be present in the same directory. The dataset contains two primary columns:
* `study_hours`: The independent variable (predictor) representing the time spent studying.
* `student_marks`: The dependent variable (target) representing the corresponding academic score.

## 🧠 Model Training Details
* **Algorithm**: Linear Regression (`sklearn.linear_model.LinearRegression`).
* **Data Splitting**: The dataset is separated into 80% training data and 20% testing data (`test_size=0.2`) using a `random_state` of 0.
* **Execution**: The model is fit using the `X_train` and `y_train` data splits.

## 🚀 Usage
When running the final cell of the notebook, the system will prompt you with: `Enter the Study Hours: `. 
* If you enter a value between 4 and 12, the script will round the predicted score to two decimal places and display `Expected Marks= [result]`. 
* If you enter a value outside of this range, it will output `Invalid Study Hours`.
