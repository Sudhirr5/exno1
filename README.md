
# 1) Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
```python
#progarm done by : R.SUDHIR KUMAR
#register number : 212223230221
```
```python
#reading csv file
import pandas as pd
df=pd.read_csv("/content/SAMPLEIDS.csv")
df
```
![pic](read.png)
```python
#finding head and tail of the data
print(df.head(5))
print(df.tail(5))
```
![pic](hf.png)
```python
#checking null values
print(df.isnull())
```
![pic](isnull.png)
```python
#filling null values with 0
print(df.fillna(0))
```
![pic](fnull.png)
```python
#total no. of null in each columns
df.isnull().sum()
```
![pic](nullsum.png)
```python
# drop axis
df.dropna(axis=1)
```
![pic](dropax.png)
```python
#describe
df.describe()
```
![pic](desc.png)
# Result
Thus, the given data is read, cleansed and the cleaned data is saved into the file and the given data is read,remove outliers and save a new dataframe was created and executed successfully.