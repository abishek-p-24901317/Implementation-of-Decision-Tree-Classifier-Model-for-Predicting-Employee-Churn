# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Loads and explores the employee dataset, checking structure and missing values.

2.Encodes categorical data and selects relevant features for modeling.

3.Splits data and trains a Decision Tree Classifier using the entropy criterion.

4.Evaluates model accuracy and predicts attrition for sample input.

5.Displays accuracy, prediction result, and user identification details.
## Program:
```
/*
import pandas as pd
data = pd.read_csv("Employee.csv")
print("HEAD DATA:")
print(data.head())
print("DATA INFO")
print(data.info())
print("NULL DATA SET")
print(data.isnull().sum())
print('VALUE COUNT ON LEFT:')
print(data['left'].value_counts())
​
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
​
data['salary'] = le.fit_transform(data['salary'])
print("DATASET TRANSFORM HEAD:")
print(data.head())
​
x=data[['satisfaction_level','last_evaluation','number_project','average_montly_hours','time_spend_company','Work_accident','promotion_last_5years','salary']]
print("X HEAD:")
print(x.head())
​
y=data['left']
​
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state =100)
​
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion='entropy')
dt.fit(x_train,y_train)
y_predict=dt.predict(x_test)
​
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_predict)
print("ACCURACY:")
print(accuracy)
print("DATA PRECICTION:")
print(dt.predict([[0.5,0.8,9,260,6,0,1,2]]))
​
*/
```

## Output:
## DATASET :
![437689499-a20b9cbc-7d29-4e1f-bb4f-74ad7ca4bf50](https://github.com/user-attachments/assets/0474b44c-d988-4c0c-9921-8abcf3b58e09)

## NULL DATASET:
![437689537-af0c39bc-eed1-408c-b2cf-2a012bb0f617](https://github.com/user-attachments/assets/798e4c77-9b27-4d28-9cae-6400cebbbb62)

## VALUE COUNT IN LEFT COLUMN:
![437689640-81204c17-13bb-49d9-a273-0eede8810e3f](https://github.com/user-attachments/assets/7f0b368a-5943-428f-bdb2-efeb4c341c49)

## DATASET TRANSFORMED HEAD:
![437689700-ed34822f-7e4d-4b63-9429-6ad404c0e76c](https://github.com/user-attachments/assets/9e5815aa-bacb-450a-9728-5851d93af410)

## X HEAD
![437689757-b0a53305-07db-44a6-aab7-d971957ab108](https://github.com/user-attachments/assets/a4e3a1f0-4287-4981-b25c-9b539f286649)

## ACCURACY
![437689798-d03511b9-1f67-45ea-b0d0-952777d09acb](https://github.com/user-attachments/assets/d5bc7962-63f5-4ac7-b409-0b5c72609654)

## DATA PREDICTION
![image](https://github.com/user-attachments/assets/c230f8fd-0643-477e-bd44-d994571d8f82)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
