# MULTIVARIANT-ANALYSIS
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Multivariant Analysis is the process of preparing data for analysis by statistical study of data where multiple measurements are made on each experimental unit and where the relationships among multivariate measurements

# ALGORITHM
# STEP 1
Read the given Data

# STEP 2
Get the information about the data

# STEP 3
Analyse Scatter plot

# STEP 4
Analyse Bar Chart

# STEP 5
Analyse Box plot

# STEP 6
Analyse HeatMap

# CODE
import pandas as pd
import seaborn as sns
import numpy as np
import matplotlib.pyplot  as plt
df=pd.read_csv("/content/SuperStore.csv")
df.head()   

sns.scatterplot(x=df['Sales'],y=df['Sub-Category'])

sns.boxplot(x="Sales",y="Sub-Category", data=df)

sns.barplot(x=df["Sales"],y=df["Sub-Category"],data=df)

sns.barplot(x=df['Region'],y=df['Sales'],hue=df['Category'])

df.corr()

sns.heatmap(df.corr(),annot=True)

# OUTPUT
![image](https://user-images.githubusercontent.com/107982953/235744009-a809811d-6a3a-4a98-9ff8-43b4dbb41205.png)
![image](https://user-images.githubusercontent.com/107982953/235744074-f84deaa9-6302-4bec-8939-45f1883a8c89.png)
![image](https://user-images.githubusercontent.com/107982953/235744129-6eae6703-0cf1-403a-a387-e25832662e2a.png)
![image](https://user-images.githubusercontent.com/107982953/235744191-ef7f03ad-8fe2-4bc2-bddd-b08feab7a89c.png)
![image](https://user-images.githubusercontent.com/107982953/235744258-a210fd9b-a5ed-4917-aa3f-185ec7d8c896.png)
![image](https://user-images.githubusercontent.com/107982953/235744322-b92dd1a0-1005-4aa3-b86c-7a918a1a5da6.png)
![image](https://user-images.githubusercontent.com/107982953/235744391-8d807eab-47c9-443e-9766-fecf893b4666.png)

# RESULT
Thus we have performed statistical analysis using multivariant analysis.
