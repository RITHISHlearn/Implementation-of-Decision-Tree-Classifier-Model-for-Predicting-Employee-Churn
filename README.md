# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries.

2.Upload and read the dataset.

3.Check for any null values using the isnull() function.

4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.

5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.


## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: RITHISH P
RegisterNumber:  212223230173
 
 
import pandas as pd

data=pd.read_csv("Employee.csv")

data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder

le=LabelEncoder()

data["salary"]=le.fit_transform(data["salary"])

data.head()

x=data[["satisfaction_level","last_evalution","number_project","average_montly_hours","time_spend_company","work_accident","promotion_last_5years","salary"]]

x.head()

y=data["left"]

from sklearn.model_selection import train_test_split

x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier

dt=DecisionTreeClassifier(criterion="entropy")

dt.fit(x_train,y_train)

y_pred=dt.predict(x_test)

from sklearn import metrics

accuracy=metrics.accuracy_score(y_test,y_pred)

accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```
## Output:
       Data.head():



       
 ![Screenshot 2024-04-03 040604](https://github.com/RITHISHlearn/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145446645/84b79b95-c067-4aef-bef5-41f3abb99b84)











 
       Data.info():


       
![Screenshot 2024-04-03 040618](https://github.com/RITHISHlearn/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145446645/e2be044f-482f-4916-bef1-9f70ee1377ca)















       isnull() and sum():






       
![Screenshot 2024-04-03 040634](https://github.com/RITHISHlearn/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145446645/0539862d-d022-4e31-be23-a80b708b8631)













       Data Value Counts():
       
![Screenshot 2024-04-03 040645](https://github.com/RITHISHlearn/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145446645/e82657a9-c4e2-4f7d-8489-c8c4ca1e68c0)









       Data.head() for salary:
       
![Screenshot 2024-04-03 040711](https://github.com/RITHISHlearn/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145446645/5b786847-502e-4060-bb3f-c9213bfde6f3)










       x.head:
       
![Screenshot 2024-04-03 040722](https://github.com/RITHISHlearn/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145446645/768976ab-3d6f-490c-8256-fa4008f6cb88)











       Accuracy Value:
       
![Screenshot 2024-04-03 040730](https://github.com/RITHISHlearn/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145446645/786301bd-f399-40c4-9e99-ab81fb021317)






       Data Prediction:
       
![Screenshot 2024-04-03 040748](https://github.com/RITHISHlearn/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/145446645/4d39b9b7-e541-4208-abd4-86df8620f094)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
