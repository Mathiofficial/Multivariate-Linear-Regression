# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

<br>Import panda as pd.

### Step2

use pd.read_csv to find weight and volume.

### Step3

Run the program and take the screenshot of the output

### Step4

End of the program

### Step5
<br>

## Program:
```


import pandas as pd
from sklearn import linear_model
df=pd.read_csv("csvfile.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('predicted co2 for the corresponding Weight and Volume',predictedCO2)





```
## Output:


### Insert your output

![Screenshot from 2023-01-24 12-58-12](https://user-images.githubusercontent.com/118787327/214237387-5883f9e2-0ecd-4d39-8c9c-4b9302dff908.png)

![Screenshot from 2023-01-24 12-57-54](https://user-images.githubusercontent.com/118787327/214237443-4ab5a481-ee02-4ff2-ab85-55c8160ee29a.png)





## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
