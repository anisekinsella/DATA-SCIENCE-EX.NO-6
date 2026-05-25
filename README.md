# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_csv("titanic_dataset.csv")
df.head()
```

<img width="1225" height="203" alt="image" src="https://github.com/user-attachments/assets/ccc149a0-1613-4283-9b3c-2e713a4b0e7c" />

```
 x=[1,2,3,4,5]
 y=[3,6,2,7,1]
 sns.lineplot(x=x,y=y)
 plt.title('Line Plot')
```

<img width="716" height="581" alt="image" src="https://github.com/user-attachments/assets/6a52f9fc-f58a-427d-925e-4b830a8dc8a2" />

```
 x=[1,2,3,4,5]
 y1=[3,5,2,6,1]
 y2=[1,6,4,3,8]
 y3=[5,2,7,1,4]
 sns.lineplot(x=x,y=y1)
 sns.lineplot(x=x,y=y2)
 sns.lineplot(x=x,y=y3)
 plt.title('Multi Line Plot')
```

<img width="706" height="572" alt="image" src="https://github.com/user-attachments/assets/65edbf0b-ef96-4006-b145-63d5decdb50c" />

```
 plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
```

<img width="747" height="542" alt="image" src="https://github.com/user-attachments/assets/34a0f8f7-f7f3-438c-96ed-cf8733486d6d" />

```
sns.scatterplot(x="Age", y="Fare", data=df)
plt.title('Scatterplot of Age vs Fare')
plt.show()
```

<img width="748" height="555" alt="image" src="https://github.com/user-attachments/assets/cabf84fd-865f-4c26-afc6-5464e2311d11" />

```
 sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
 plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
 plt.show()
```

<img width="742" height="557" alt="image" src="https://github.com/user-attachments/assets/5140c270-327d-4934-be1c-095bc4a63071" />

```
 sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```

<img width="728" height="576" alt="image" src="https://github.com/user-attachments/assets/9a9310df-64e1-43ec-be65-01d887fc6bcd" />

```
 sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
 plt.title("Age By Passenger Class")
```

<img width="722" height="606" alt="image" src="https://github.com/user-attachments/assets/10d81589-b5a6-4922-9f0a-056937dbd6d8" />

```
 sns.violinplot(x="Pclass", y="Fare", data=df)
 plt.title('Violin Plot of Fare by Passenger Class')
 plt.show()
```

<img width="748" height="562" alt="image" src="https://github.com/user-attachments/assets/57854bd2-ba6e-4d3b-8700-0f823ff1a413" />

```
 sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
```

<img width="758" height="568" alt="image" src="https://github.com/user-attachments/assets/cdee44bb-10ec-4163-a3b1-fda1e175dea4" />

```
 numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
```

<img width="753" height="616" alt="image" src="https://github.com/user-attachments/assets/9d0e3480-c94a-4629-a700-381397f091d7" />


# Result:
Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
