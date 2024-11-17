# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the necessary python packages using import statements.

2.Read the given csv file using read_csv() method and print the number of contents to be displayed using df.head().

3.Split the dataset using train_test_split.

4.Calculate Y_Pred and accuracy.

5.Print all the outputs.

6.End the Program. 

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: DEVA DHARSHINI I
RegisterNumber: 212223240026
import chardet
file='spam.csv'
with open (file,'rb') as rawdata:
    result = chardet.detect(rawdata.read(100000))
result

import pandas as pd
data=pd.read_csv("spam.csv",encoding='windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values
y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
## ENCODING:
![Screenshot 2024-11-17 115440](https://github.com/user-attachments/assets/16ecafc1-50a6-4603-a9bd-7fa768397f30)
## HEADING:
![Screenshot 2024-11-17 115535](https://github.com/user-attachments/assets/152360c2-c080-4a19-b952-b12998920fc8)
## INFO:
![Screenshot 2024-11-17 115550](https://github.com/user-attachments/assets/c7a83370-c2de-4f07-bcd6-6a9353f00eb7)
## isnull().sum():
![Screenshot 2024-11-17 115646](https://github.com/user-attachments/assets/7719cae0-fd72-40c2-bade-236790d1ff43)
## prediction of y:
![Screenshot 2024-11-17 115659](https://github.com/user-attachments/assets/a418fe47-463f-4c40-a060-dd9056536084)
## ACCURACY:
![Screenshot 2024-11-17 115710](https://github.com/user-attachments/assets/0c7cab16-1892-48e7-9b36-d51689a29726)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
