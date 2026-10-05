# Student Performance Prediction using Machine Learning

## 📌 Project Overview

This project predicts a student's **Final Score** based on academic performance-related factors such as study hours, attendance, previous score, and assignments completed.

The project is implemented in **Python using Google Colab** and uses machine learning regression algorithms to predict and compare student performance.

## 🎯 Objective

The main objectives of this project are:

* Create a student performance dataset.
* Explore and understand the dataset.
* Check for missing values.
* Separate features and target variables.
* Split the dataset into training and testing data.
* Train multiple machine learning regression models.
* Predict students' final scores.
* Evaluate and compare the performance of the models.

## 📊 Dataset

The dataset contains **15 student records** and the following columns:

| Feature                 | Description                       |
| ----------------------- | --------------------------------- |
| `Study_Hours`           | Number of hours studied           |
| `Attendance`            | Student attendance percentage     |
| `Previous_Score`        | Student's previous academic score |
| `Assignments_Completed` | Number of assignments completed   |
| `Final_Score`           | Student's final score             |

### Target Variable

`Final_Score` is the target variable that the models try to predict.

## 🤖 Machine Learning Models

Three regression models are used:

### 1. Decision Tree Regressor

A Decision Tree Regressor predicts the final score by creating decision-based splits from the input features.

### 2. Random Forest Regressor

Random Forest combines multiple decision trees to produce a more reliable prediction.

### 3. Regression Tree

A Decision Tree Regressor with a maximum depth of 3 is also trained and evaluated.

## 🔄 Project Workflow

```text
Create Dataset
      ↓
Explore Dataset
      ↓
Check Missing Values
      ↓
Separate Features and Target
      ↓
Train-Test Split
      ↓
Train Machine Learning Models
      ↓
Generate Predictions
      ↓
Evaluate Models
      ↓
Compare Model Performance
```

## 🛠️ Technologies Used

* Python
* Google Colab
* Pandas
* Scikit-learn
* Machine Learning
* Decision Tree
* Random Forest

## 📦 Libraries Used

```python
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeRegressor
from sklearn.ensemble import RandomForestRegressor
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
```

## 📈 Model Evaluation

The models are evaluated using:

### MAE — Mean Absolute Error

Measures the average absolute difference between the actual and predicted values.

**Lower MAE is better.**

### MSE — Mean Squared Error

Measures the average squared difference between actual and predicted values.

**Lower MSE is better.**

### R² Score

Measures how well the model explains the variation in the target variable.

**Higher R² is better.**

## 🏆 Results

The notebook produced the following results:

| Model           |    MAE |     MSE | R² Score |
| --------------- | -----: | ------: | -------: |
| Decision Tree   | 3.6667 | 16.3333 |   0.8061 |
| Random Forest   | 1.2900 |  2.4215 |   0.9712 |
| Regression Tree | 4.5556 | 22.2593 |   0.7357 |

Based on these results, the **Random Forest Regressor** achieved the best performance among the three models, with the lowest MAE and MSE and the highest R² score.

## 🚀 How to Run the Project

### Using Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `ML_MODEL.ipynb`.
3. Open the notebook.
4. Run the cells from top to bottom.
5. Observe the dataset, predictions, evaluation metrics, and model comparison.

### Using Jupyter Notebook

Install the required libraries:

```bash
pip install pandas scikit-learn
```

Then open:

```text
ML_MODEL.ipynb
```

and run the notebook cells.

## 📁 Project Structure

```text
Student-Performance-Prediction/
│
├── ML_MODEL.ipynb
├── student_performance.csv
└── README.md
```

## 🔮 Future Improvements

This project can be improved by:

* Using a larger real-world student dataset.
* Adding more student-related features.
* Performing feature engineering.
* Using cross-validation.
* Hyperparameter tuning.
* Adding visualization and graphs.
* Testing additional regression algorithms.
* Creating a user interface where users can enter student information and receive a predicted final score.

## 👩‍💻 Conclusion

This project demonstrates how machine learning regression algorithms can be used to predict student final scores from academic performance features.

Among the tested models, the **Random Forest Regressor performed best on the notebook's test split**, achieving an R² score of approximately **0.9712**.

> **Note:** The dataset is small, containing only 15 records, so the reported performance should not be considered representative of performance on a larger real-world dataset.
