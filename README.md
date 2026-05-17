# Student Math Score Prediction using PyTorch

## Problem Description

This project builds a Deep Learning Regression model using PyTorch to predict students' math scores based on different student-related features from the dataset.

The project includes:

* Data preprocessing
* Handling missing values
* Encoding categorical variables
* Feature scaling
* Splitting dataset into training, validation, and testing sets
* Building multiple neural network models
* Training and validation
* Model evaluation and comparison

The task is a **Regression Problem** because the target variable (`math_score`) contains continuous numerical values.

---

# Dataset

Dataset File Used:

* `stud.csv`

Dataset Link:

https://www.kaggle.com/datasets/fatimariazz/student-performance-prediction

Example:


/content/stud.csv

---

# Libraries Used

The project uses the following Python libraries:

python
torch
numpy
pandas
matplotlib
scikit-learn


Install dependencies using:


pip install torch numpy pandas matplotlib scikit-learn


---

# Project Workflow

## 1. Load Dataset

The dataset is loaded using Pandas.

## 2. Handle Missing Values

Missing numerical values are filled using the mean value of each column.

## 3. Define Target Variable

The target variable is:

math_score


## 4. Split Dataset

The dataset is divided into:

* Training Set
* Validation Set
* Test Set

## 5. Encoding

Categorical features are converted into numerical values using One-Hot Encoding.

## 6. Feature Scaling

Features are normalized using `StandardScaler`.

## 7. Convert Data to PyTorch Tensors

Data is converted into tensors for PyTorch model training.

## 8. Build Neural Network Models

Three different neural network models are created and tested.

## 9. Training

Models are trained using:

* Adam Optimizer
* MSE Loss Function

## 10. Evaluation

Models are evaluated using:

* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)
* R-squared Score (R2)

---

# Models Architecture

## Model 1

* Input Layer → 16 Neurons
* Hidden Layer → 8 Neurons
* ReLU Activation
* Dropout = 0.3
* Learning Rate = 0.01

## Model 2

* Input Layer → 32 Neurons
* Hidden Layer → 32 Neurons
* ReLU Activation
* Dropout = 0.3
* Learning Rate = 0.001

## Model 3

* Input Layer → 16 Neurons
* Hidden Layer → 8 Neurons
* ReLU Activation
* Dropout = 0.3
* Learning Rate = 0.001

---

# Results

| Model   | Activation | Learning Rate | MSE         | MAE       | R2         |
| ------- | ---------- | ------------- | ----------- | --------- | ---------- |
| Model 1 | ReLU       | 0.010         | 121.626427  | 9.206055  | 0.500176   |
| Model 2 | ReLU       | 0.010         | 1512.320435 | 36.908302 | -5.214886  |
| Model 3 | ReLU       | 0.001         | 3887.241943 | 60.546585 | -14.974634 |

---

# Best Model

Model 1 achieved the best performance because:

* Lowest MSE
* Lowest MAE
* Highest R2 Score

This means Model 1 predicts student math scores more accurately than the other models.

---

# Visualization

The project includes:

* Training vs Validation Loss graphs
* Model comparison bar chart

These visualizations help analyze model performance and overfitting.

---

# Instructions for Running the Project



## Step 1: Install Required Libraries

pip install torch numpy pandas matplotlib scikit-learn


---

## Step 2: Add Dataset

Place the dataset file:

stud.csv

inside the project folder.

---

## Step 3: Run the Project

Run the Python script or Jupyter Notebook:

python project.py

---

# Output

The project outputs:

* Training and validation losses
* Evaluation metrics
* Comparison table
* Performance graphs

---

# Conclusion

This project demonstrates how Deep Learning can be used for regression tasks using PyTorch.

Different neural network architectures and learning rates were tested to compare their performance.

Model 1 produced the best prediction results for student math score prediction.
