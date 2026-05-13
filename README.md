# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1. Data Loading: Import the dataset and convert text labels (like Salary) into numbers.

2. Data Splitting: Divide the data into Features (X) and Target (y), then split into Training and Testing sets.

3. Model Training: Build the DecisionTreeClassifier using the Entropy criterion and train it with the training data.

4. Evaluation: Predict outcomes for the test set, calculate Accuracy, and visualize the results via a Confusion Matrix.


## Program:
```python
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier, plot_tree
from sklearn.metrics import accuracy_score
data = pd.read_csv("Employee.csv")
data = pd.get_dummies(data, drop_first=True)
X = data.iloc[:, :-1]
y = data.iloc[:, -1]
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
model = DecisionTreeClassifier(random_state=42)
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
print("Accuracy:", accuracy_score(y_test, y_pred))
plt.figure(figsize=(20,10))

plot_tree(
    model,
    feature_names=X.columns,
    filled=True
)

plt.show()

Developed by: JINITH KUMAR V
RegisterNumber:  212225040157
*/
```

## Output:
<img width="1290" height="674" alt="image" src="https://github.com/user-attachments/assets/d5d4826d-bccb-4218-99ee-e817383f75e7" />



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
