# Ex:-01(DATA CLEANSING)

## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

## EXPLANATION
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

## ALGORITHM
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

## PROGRAM
```python3
import pandas as pd 
df=pd.read_csv("Data_set.csv") 
print(df) 
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0]) 
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0]) 
df['original_network']=df[ 'original_network'].fillna(df['aired_on'].mode()[0]) 
df.head()
df['rating']=df['rating'].fillna (df['rating'].mean()) 
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean()) 
df.head()
df['watchers']=df['watchers'].fillna (df['watchers'].median()) 
df.head()
df.info()
df.isnull().sum()
import pandas as pd 
df=pd.read_csv("Loan_data.csv") 
print(df) 
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['Loan_ID']=df['Loan_ID'].fillna(df['LoanAmount'].mode()[0]) 
df.head()
df['Dependents']=df['Dependents'].fillna (df['Dependents'].mode()[0]) 
df.head()
df['Gender']=df['Gender'].fillna (df['Gender'].mode()[0]) 
df.head()
df['Education']=df['Education'].fillna (df['Dependents'].mode()[0]) 
df.head()
df['Self_Employed']=df['Self_Employed'].fillna (df['Self_Employed'].mode()[0]) 
df.head()
df['LoanAmount']=df['LoanAmount'].fillna (df['LoanAmount'].mean()) 
df.head()
df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].mean()) 
df.head()
df['Credit_History']=df['Credit_History'].fillna (df['Credit_History'].median()) 
df.head()
df.info()
f.isnull().sum()
```
## OUTPUT

![1](https://github.com/Shinysudhakar/expno1ds/assets/127575325/a5073e8d-648c-473b-994e-d08685c2b62d)![2](https://github.com/Shinysudhakar/expno1ds/assets/127575325/228e4236-71b6-4c92-b649-cae0ee657f2b)
![3](https://github.com/Shinysudhakar/expno1ds/assets/127575325/24211940-6a37-4861-a27a-4e1477dc501c)

![4](https://github.com/Shinysudhakar/expno1ds/assets/127575325/9cd408f8-a987-41ef-9c5e-94a3b85f0fbb)
![5](https://github.com/Shinysudhakar/expno1ds/assets/127575325/6c4e600b-b19b-4aa8-859e-e0cd8cd2a9f6)

![6](https://github.com/Shinysudhakar/expno1ds/assets/127575325/e0f334c2-5a73-4957-9596-e0df3d2dfaea)

![7](https://github.com/Shinysudhakar/expno1ds/assets/127575325/109c092b-4ac5-43e8-9fbd-88d2d6fedb43)
![8](https://github.com/Shinysudhakar/expno1ds/assets/127575325/019ca09b-985f-4d87-ae66-3144abeee6f2)

![9](https://github.com/Shinysudhakar/expno1ds/assets/127575325/77fd580c-baca-4ef2-8d5f-286b6aaa922a)

![10](https://github.com/Shinysudhakar/expno1ds/assets/127575325/7b62edb0-2c46-4c4a-ad4f-c21b14b74c0e)


![11](https://github.com/Shinysudhakar/expno1ds/assets/127575325/4a5025da-c7b8-4549-95ba-2e8570ff4dfd)


![12](https://github.com/Shinysudhakar/expno1ds/assets/127575325/6c9f7a24-df80-4a8a-b0c7-ecdfc52e3750)







