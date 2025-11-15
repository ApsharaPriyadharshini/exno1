# Exno:1
Data Cleaning Process

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
import pandas as pd
data=pd.read_csv("Data_Set.csv")
print(data)

<img width="825" height="551" alt="{2696F022-539E-4FFF-A187-4E259667A10C}" src="https://github.com/user-attachments/assets/940511f6-dafb-496f-9c49-9b3dc64bf47e" />

<img width="788" height="317" alt="{6F69B9A2-202D-4ADF-887B-A1DA60F0B325}" src="https://github.com/user-attachments/assets/42b3b6dd-6583-4b98-9554-0179a505a71a" />

df=pd.DataFrame(data)
print(df)

<img width="976" height="553" alt="image" src="https://github.com/user-attachments/assets/1127ed44-56a4-4c1d-ab20-b67e71357a65" />

<img width="474" height="321" alt="{1A02361B-57EC-4DAD-B5BA-3374830A39FC}" src="https://github.com/user-attachments/assets/ad382333-3e2f-4a8a-af69-a09b2900d204" /> 

df.describe()

<img width="754" height="311" alt="image" src="https://github.com/user-attachments/assets/bfad6d47-9bca-4aba-ab2f-2ecafd701c3c" />

df.info()

<img width="577" height="357" alt="image" src="https://github.com/user-attachments/assets/0509d54e-9147-4c16-8d37-96b0d1e710a5" />

df.isna()

<img width="1107" height="429" alt="{2C25E21A-2ECE-4E82-81BE-A22E4BC5EDB8}" src="https://github.com/user-attachments/assets/3b47b0d8-8d7c-447a-bf51-5a283358a8d6" />

df.isna().sum()

<img width="342" height="229" alt="image" src="https://github.com/user-attachments/assets/1e3cf8dd-07cd-4923-9983-6b19aeb2a5ff" />

df.duplicated()

<img width="332" height="283" alt="image" src="https://github.com/user-attachments/assets/1c905c61-a542-4195-b0be-d8acb76e6b95" />

df.drop_duplicates()

<img width="1243" height="609" alt="{90EF3E4C-EC39-4A55-81FD-4C5F2553E888}" src="https://github.com/user-attachments/assets/2e4ddff4-3e6a-49a1-b10b-e2b1e15e97b1" />

df.dropna()

<img width="1251" height="595" alt="{EF7189A8-5379-4C34-B7AE-00945462B7D9}" src="https://github.com/user-attachments/assets/d760d756-b328-429e-96a2-a9a06f015452" />

df.dropna(axis=0,inplace=True)

df.dropna(axis=1,inplace=True)

print(df)

<img width="752" height="552" alt="{6D722EA6-BF1C-4B67-8097-7E68130EC0A7}" src="https://github.com/user-attachments/assets/cbea9fd0-d7a2-4b9f-95be-fe3b8dbbef16" />

<img width="496" height="336" alt="image" src="https://github.com/user-attachments/assets/b758d9de-ebe4-4080-b416-ef886e153a33" />

df.fillna(0)

<img width="1247" height="610" alt="{E4A7A375-260F-4167-AEA2-487113E49E02}" src="https://github.com/user-attachments/assets/7661c296-c0fe-4ce9-9da2-4a86ba340bc4" />

df.ffill()

<img width="1249" height="600" alt="{5EC8A731-2324-425B-87DA-8D3DC22A9344}" src="https://github.com/user-attachments/assets/a23646b1-18c8-4b90-97f5-d361d68c9e5f" />

df.bfill()

<img width="1237" height="612" alt="{728DCB01-9137-4DDC-B18C-5056A7C63FA1}" src="https://github.com/user-attachments/assets/5309c083-d193-4a1c-bb39-c70b90862783" />




















# Result
          <<include your Result here>>
