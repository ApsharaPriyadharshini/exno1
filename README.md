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

import pandas as pd
data=pd.read_csv("Data_Set.csv")
print(data)
<img width="1274" height="572" alt="{A2B65C5E-0E14-491D-8478-946CA5F0C3C3}" src="https://github.com/user-attachments/assets/3cbe3e09-7a4e-4f79-9619-6e1f3459d427" />
<img width="1280" height="315" alt="{58D32930-425C-4A3D-8C2F-66F273E81D9E}" src="https://github.com/user-attachments/assets/7748359e-6948-496c-be4d-f3ea4d265649" />

df=pd.DataFrame(data)
print(df)
<img width="1260" height="548" alt="{8A928D6C-4E4C-401C-8B05-6D700CDC2C61}" src="https://github.com/user-attachments/assets/6e61753a-b5b3-4589-b4f1-78b07774d6b2" />
<img width="1248" height="315" alt="{A45EE093-BA6E-41A6-98F7-55AC7922127D}" src="https://github.com/user-attachments/assets/e8a18a85-f665-4c8b-8d2d-fc923e7a8e50" />

df.fillna(0)
<img width="1265" height="444" alt="image" src="https://github.com/user-attachments/assets/07a1cd23-f605-49b3-bc77-118aca07fe19" />


df.ffill()
<img width="1246" height="445" alt="{959927ED-AF9D-4680-BFB5-7555B63A591B}" src="https://github.com/user-attachments/assets/9701eb42-f814-4523-ae68-1a51d87efe60" />

df.bfill()
<img width="1277" height="453" alt="image" src="https://github.com/user-attachments/assets/766b3d11-ed9d-4063-aba0-fc2e13b9900a" />

import pandas as pd
import numpy as np
from scipy import stats
import seaborn as sns
ir=pd.read_csv('iris.csv')
ir
<img width="651" height="440" alt="{C2058DA5-79D4-4E71-AA7D-AE7054C14C3F}" src="https://github.com/user-attachments/assets/47532f5b-0272-4754-9592-2afdfb313180" />

sns.boxplot(ir)
<img width="751" height="559" alt="{4919CB20-DC59-4B02-BCBD-2F9E51ABB730}" src="https://github.com/user-attachments/assets/743fda30-0385-4398-8e05-9a4ee2231dcf" />

sns.scatterplot(ir)
<img width="844" height="563" alt="{2C381C13-7EC0-4422-ABAD-9872DCD1BC93}" src="https://github.com/user-attachments/assets/567b4da3-20be-4cdf-8128-f0be41343759" />

q1=ir.sepal_width.quantile(0.25)
q3=ir.sepal_width.quantile(0.75)
iqr=q3-q1
print(iqr)
<img width="988" height="37" alt="image" src="https://github.com/user-attachments/assets/048aa514-2abf-4917-8c6d-00761c56913c" />

rid=ir[((ir.sepal_width<(q1-1.5*iqr))|(ir.sepal_width>(q3+1.5*iqr)))]
rid['sepal_width']
<img width="422" height="128" alt="image" src="https://github.com/user-attachments/assets/87bfd677-39f0-4519-a126-fcbc60c96b94" />

delid=ir[~((ir.sepal_width<(q1-1.5*iqr))|(ir.sepal_width>(q3+1.5*iqr)))]
delid
<img width="678" height="454" alt="{6BA3CB27-42E3-4668-8B57-23FBA24E5E57}" src="https://github.com/user-attachments/assets/6fb2b50a-0421-4fe9-8a56-e182b1b72bee" />

data=[1,12,15,18,21,24,27,30,33,36,39,42,45,48,51,54,57,60,63,66,69,72,75,78,81,84,87,90,93]
df=pd.DataFrame(data)
mean=np.mean(data)
mean
<img width="628" height="42" alt="{D6D7DB45-B579-4387-9D11-4C0084A218E7}" src="https://github.com/user-attachments/assets/d21e1d43-b21c-479b-a33c-88e8e3d919a1" />

std=np.std(data)
std
z=np.abs(stats.zscore(df))
z
<img width="204" height="760" alt="{2B609550-4052-460D-A2F3-54B875A8B9E2}" src="https://github.com/user-attachments/assets/bbf80dba-584a-468c-9658-58ee80482a9e" />
<img width="223" height="200" alt="image" src="https://github.com/user-attachments/assets/997bb1ce-5dbd-4817-afdd-c11e40439eee" />

threshold=3
outliers=df[abs(df)>3]
print("Outliers:")
print(outliers)
<img width="1116" height="672" alt="{43AABDD7-A6AF-41B0-8F36-E06B7925C475}" src="https://github.com/user-attachments/assets/a6828e3d-2208-4279-85e9-84cde5c2f0fa" />

df_cleaned=df[z<=threshold]
df_cleaned
<img width="1238" height="736" alt="{023C33FE-0537-4EC2-82C9-06DE3FB43520}" src="https://github.com/user-attachments/assets/a917fc58-4085-41c7-a449-75d0228fd6bd" />
<img width="1143" height="239" alt="image" src="https://github.com/user-attachments/assets/1fbdbc82-24df-4c20-8c6a-fec9053571cb" />

                    
# Result
          Thus, the data has been cleaned and outliers has been removed by detection using IQR and Z-score method.
