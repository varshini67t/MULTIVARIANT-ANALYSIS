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

# RESULT
Thus we have performed statistical analysis using multivariant analysis.
