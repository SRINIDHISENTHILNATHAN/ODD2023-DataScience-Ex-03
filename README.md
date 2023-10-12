# ODD2023-DataScience-Ex-03
# Aim:
To read the given data and perform the univariate analysis with different types of plots.

# Explanation:

### Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:
### Step1: Read the given data.
### Step2: Get the information about the data.
### Step3: Remove the null values from the data.
### Step4: Mention the datatypes from the data.
### Step5: Count the values from the data.
### Step6: Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:
```
Developed By: SRINIDHI SENTHIL
Register Number: 212222230148
```
# Diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("/content/diabetes.csv exp3.csv")
df
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/0d7ec488-9360-4f1b-a769-8032144ff023)
```
df.head()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/66f55ba4-5c5e-4217-b36d-0e715fe26609)
```
df.info()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/3467c089-860e-46a0-9418-d528e37babd9)
```
df.describe()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/209da76b-8953-463a-998d-588b4a661d5b)
```
df.isnull().sum()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/898090e6-d5d4-47d1-9150-ffc4dc7693f7)
```
df.dtypes
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/600a1c5d-7126-4f2b-a718-650bb5e34b98)
```
df['BMI'].value_counts()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/06a678c4-ca9b-4edd-a98e-f01b83003dd9)
```
sns.boxplot(x="BMI", data=df)
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/7328834e-aa73-4435-9a4a-15fb65479fc1)
```
sns.countplot(x="BMI", data=df)
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/cbf14c0c-963d-4d21-9051-9d12c9fb0db9)
```
sns.distplot(df["BMI"])
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/79dba318-63ba-47e6-add6-3ad115d4362d)
```
sns.histplot(x="BMI", data=df)
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/932a5cc7-a7c9-425c-b653-49902e1134b3)

# SuperStore
