# ODD2023-DataScience-Ex-03
# AIM:
To read the given data and perform the univariate analysis with different types of plots.

# EXPLANATION:

### Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# ALGORITHM:
### Step1: Read the given data.
### Step2: Get the information about the data.
### Step3: Remove the null values from the data.
### Step4: Mention the datatypes from the data.
### Step5: Count the values from the data.
### Step6: Do plots like boxplots,countplot,distribution plot,histogram plot.

# PROGRAM:
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

# emplyeesal.csv
```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv("/content/employeesal.csv exp3.csv")
df
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/68ab6f77-626e-478f-8c58-4ea8b4e58e0d)
```
df.head()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/043254e3-4416-4a2f-872d-51f25f51f6f9)
```
df.info()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/740dc89a-4ed0-4628-8a54-b4a56a54c218)
```
df.describe()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/f9ed7cdf-3b06-42f6-8452-62518ede0545)
```
df.isnull().sum()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/b668364c-af69-4844-897e-58a557a96895)
```
df.dtypes
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/5eed451f-1ab7-4c49-9d4f-07242bcc898b)
```
df['Salary'].value_counts()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/4f4852e5-13dd-458f-830d-79f77fc9f25f)
```
sns.boxplot(x="Salary", data=df)
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/4e6a06f4-0de2-4bd2-8d73-82baac08f99e)
```
sns.countplot(x="Salary", data=df)
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/658675f4-920d-4e09-9fb8-4dbacf8178cf)
```
sns.distplot(df["Salary"])
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/4e6a7a32-d83f-4ff7-86eb-cc95966cb9d9)
```
sns.histplot(x="Salary", data=df)
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/d74db76f-bd03-479b-aa11-683d0ba01098)
# superstore.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("/content/SuperStore.csv exp3.csv")
df
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/d0c3cd3f-ee22-4c15-91bc-833161442355)
```
df.head()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/c9be8b9b-0e23-42a9-ae89-ab1a04e933f7)
```
df.info()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/6d08a445-9437-4afa-8f93-2c6031c57549)
```
df.describe()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/f3d1be37-2499-4035-9f07-45e05beb9cec)
```
df.isnull().sum()
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/34ddbd02-5b32-4eab-9d7d-b405076bd61e)
```
df.dtypes
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/df731fdd-4cef-40ee-8f2d-7a165aa335d6)

```
df['Postal Code'].value_counts()
```
```
sns.boxplot(x="Postal Code", data=df)
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/3121a1a8-e614-450d-aaf1-05262157393e)
```
sns.countplot(x="Postal Code", data=df)
```
```
sns.distplot(df["Postal Code"])
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/8bfa3dc1-20d1-48fa-b386-4b8106b2f94a)
```
sns.histplot(x="Postal Code", data=df)
```
![image](https://github.com/SRINIDHISENTHILNATHAN/ODD2023-DataScience-Ex-03/assets/121373170/4d6c4e17-7b96-4923-ade2-93c01c750407)

# Result:
Thus we have read the given data and performed the univariate analysis with different types of plots.
