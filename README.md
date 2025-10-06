# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2. Import Decision tree classifier
3. Fit the data in the model
4. Find the accuracy score 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Divya Dharshini S
RegisterNumber: 212224240039
import pandas as pd
from sklearn import metrics
from sklearn.metrics import r2_score
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data["Salary"]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
y_pred
r2=metrics.r2_score(y_test,y_pred) 
*/
```

## Output:
<img width="271" height="191" alt="Screenshot 2025-10-06 102325" src="https://github.com/user-attachments/assets/244d17f0-0283-4f46-bd1a-6079d458f149" />

<img width="356" height="176" alt="Screenshot 2025-10-06 102332" src="https://github.com/user-attachments/assets/9e682576-c556-4b39-be66-add87046bfc2" />

<img width="166" height="88" alt="Screenshot 2025-10-06 102343" src="https://github.com/user-attachments/assets/f46577ac-357c-431d-b19b-afed80fb4df3" />

<img width="260" height="191" alt="Screenshot 2025-10-06 102350" src="https://github.com/user-attachments/assets/97702843-dee6-4566-a0ce-449fb87cc537" />

<img width="208" height="192" alt="Screenshot 2025-10-06 102358" src="https://github.com/user-attachments/assets/6d219306-374f-4d18-87df-2dee853ac7e2" />

<img width="259" height="117" alt="Screenshot 2025-10-06 102404" src="https://github.com/user-attachments/assets/d9b5fd8f-a892-4e42-830a-852a6bcfc251" />

<img width="198" height="24" alt="Screenshot 2025-10-06 102409" src="https://github.com/user-attachments/assets/721a4146-741c-49ce-857e-2d3f1064f555" />

<img width="175" height="38" alt="Screenshot 2025-10-06 102415" src="https://github.com/user-attachments/assets/9ec69630-c65f-46d9-8a2e-a344940e0280" />

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
