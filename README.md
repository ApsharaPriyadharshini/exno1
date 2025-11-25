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
<img width="960" height="553" alt="{8C7ADB9D-7917-4519-B959-6C494D142DDB}" src="https://github.com/user-attachments/assets/c8e15d5d-0091-45e1-bb43-884ca013578a" />
<img width="880" height="333" alt="{83719C40-EBBD-4934-AE76-C9161461F5E2}" src="https://github.com/user-attachments/assets/2d4ab867-5c3a-4947-a9b3-7e953001d67e" />

df=pd.DataFrame(data)
print(df)
<img width="955" height="540" alt="image" src="https://github.com/user-attachments/assets/5ec80cf5-bde9-4ac0-a6f9-beac33cbc1e0" />
<img width="918" height="325" alt="image" src="https://github.com/user-attachments/assets/34301e28-0c84-41e5-a575-44ef0b2fbf56" />

df.describe()
<img width="829" height="300" alt="{FF09CCB5-5D16-45DD-BDCE-96E9F44267B5}" src="https://github.com/user-attachments/assets/46a96f3b-70e5-4296-a02c-40231b235fa5" />

df.info()
<img width="727" height="350" alt="image" src="https://github.com/user-attachments/assets/ee053556-1b3b-4689-982d-2b9291305a31" />

df.isna()
<img width="1087" height="433" alt="image" src="https://github.com/user-attachments/assets/d12c05d7-851c-4f21-87e4-56201dfc721e" />

df.isna().sum()
<img width="745" height="239" alt="image" src="https://github.com/user-attachments/assets/1e64a583-4ec0-436c-85e5-9c41b74a5693" />

df.duplicated()
<img width="637" height="273" alt="image" src="https://github.com/user-attachments/assets/ed7535da-5c74-4465-a8e5-8a713ee97649" />

df.dropna()
<img width="1257" height="611" alt="{79C36263-3E47-4ED7-B967-C8EA610187C7}" src="https://github.com/user-attachments/assets/77f6234c-6983-4814-adc4-6b3aa7e466ec" />

df.dropna(axis=0,inplace=True)
df.dropna(axis=1,inplace=True)
df.drop_duplicates()
<img width="1251" height="617" alt="{257F2C77-461C-4705-9F27-26FD42BE05AE}" src="https://github.com/user-attachments/assets/849e8253-292f-495b-a9db-ec2fc48bd3ef" />

print(df)
<img width="819" height="554" alt="{8F8530CA-3F99-41D7-B181-DBBA9630BCF8}" src="https://github.com/user-attachments/assets/7f298fc6-5082-43ba-9c45-a6d8cf4e2539" />
<img width="766" height="321" alt="image" src="https://github.com/user-attachments/assets/4ac62a06-d638-484b-996f-268b57ea2a76" />

df.fillna(0)
<img width="1256" height="607" alt="{6DF8C21B-98EA-42A5-8C08-A6D497AD460F}" src="https://github.com/user-attachments/assets/eee2594a-dd00-4d9c-b68e-85a16ae0d258" />

df.ffill()
<img width="1280" height="594" alt="{3DFA562A-EA45-4B87-A518-F84002D50C26}" src="https://github.com/user-attachments/assets/4e58e712-658d-44e1-abf9-a0f5ab5951d3" />

df.bfill()
<img width="1260" height="600" alt="{2F042E11-C5AD-4DB8-806C-73F22F8E72E5}" src="https://github.com/user-attachments/assets/4df9b05e-ea92-45a6-8e64-d0e96a96bc1b" />

















                    
# Result
          
