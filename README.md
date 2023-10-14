# Data_Cleaning
## Ex-01_DS_Data_Cleaning
## AIM
    To read the given data and perform data cleaning and save the cleaned data to a file.
## EXPLANATION
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect,
incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data, but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

## ALGORITHM
STEP 1: Read the given Data 

STEP 2: Get the information about the data 

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

## CODE and OUTPUT
## DATA SET
~~~
import pandas as pd
df=pd.read_csv("Data_set.csv")
print(df)
df.head(10)
df.info()
df.isnull()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
df['aired_on']=df['aired_on'].fillna (df['aired_on'].mode()[0])
df['original_network']=df[ 'original_network'].fillna (df['aired_on'].mode()[0])
df.head()
df['rating']=df['rating'].fillna (df['rating'].mean())
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()
df['watchers']=df['watchers'].fillna (df['watchers'].median())
df.head()
df.info()
df.isnull().sum()
~~~
## LOAN DATA
~~~
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
df.isnull().sum()
~~~
## OUTPUT
## DATA SET
## DATA
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/4b2d1c5a-f742-4026-9727-a78771934d19)


## NON NULL BEFORE
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/31421436-f145-40f5-9d32-112a4af6d38c)


## NON NULL AFTER
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/fc647cd5-b57c-4a44-ac0a-5715a8d40c5e)


## LOAN DATA
## DATA
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/80a83491-9470-44a7-b21c-46555008f40d)


## NON NULL BEFORE
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/ed4676c2-578e-4351-8955-8aec014df901)


## MODE
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/13ba72c2-f5b6-4422-bffe-874d0b0d7909)


## MEAN
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/1f2667e0-e0b0-4740-90db-06f29f20ef84)

![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/e8e9d513-8d0a-4003-bee0-7041a010b06e)

![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/abbea89a-a96d-44a4-a98e-1c2d4750b040)

![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/a7dc9188-7b38-44f9-8af0-ed854d6e746d)

## MEDIAN
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/d8cb6988-7d73-4db5-ba19-88c2f9d96093)

![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/dfcfc043-62eb-4423-949f-70d865e42ce9)


## NON NULL AFTER
![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/4bab6a96-deb6-4f05-b44c-d1b57419b746)

![image](https://github.com/Kulaganachi/Data_cleansing/assets/133641126/28f58f6f-7ac4-4802-9db4-ba2984251558)

## RESULT
    Thus the given data is read,cleansed and the cleaned data is saved into the file.

