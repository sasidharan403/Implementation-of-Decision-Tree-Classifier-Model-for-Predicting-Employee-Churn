# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries.
2. Upload and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
5. Find the accuracy of the model and predict the required values by importing the required module from sklearn. 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: A.sasi dharan
RegisterNumber: 212221240049

import pandas as pd
data = pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["salary"] = le.fit_transform(data["salary"])
data.head()
x = data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y = data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt = DecisionTreeClassifier(criterion = "entropy")
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
### Data Head:
![ml 5 1](https://user-images.githubusercontent.com/94154712/173533871-9fed54ee-aa13-42f4-8c83-625fb5b01437.png)
### Information:
![ml5 2](https://user-images.githubusercontent.com/94154712/173534003-cf02fd7b-fe07-4bf5-b8e1-e754fceee364.png)
### Null dataset:
![ml5 3](https://user-images.githubusercontent.com/94154712/173534591-ecf2097d-1ac9-41dc-a173-9fee207f3341.png)

### Value_counts():
![ml5 4](https://user-images.githubusercontent.com/94154712/173535050-d16de990-b9a1-49d1-a734-db9372dfb065.png)

### Data Head:
![ml5 5](https://user-images.githubusercontent.com/94154712/173535382-d818370e-9bc2-4df1-a4fc-d21b8123e8c9.png)

### x.head():
![ml5 6](https://user-images.githubusercontent.com/94154712/173535413-1755e94e-7c5b-49be-9f79-8ca85af4e056.png)

#### Accuracy:
![ml5 7](https://user-images.githubusercontent.com/94154712/173535453-60ebaca8-e556-4de3-b638-446c7deca297.png)
### Data Prediction:
![ml5 8](https://user-images.githubusercontent.com/94154712/173535522-67b16d7e-3dc5-4880-b1fb-1eaf8d7c89c7.png)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
