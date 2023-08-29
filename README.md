# exp no 1 ds

Ex:-01(DATA CLEANSING)

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
python3
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

## OUTPUT
