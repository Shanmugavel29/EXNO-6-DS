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
 Include the necessary coding and corresponding screenshots
 ```
 NAME : SHANMUGAVEL RM
 REG NO : 212222230142
```

```python
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 df=pd.read_csv("titanic_dataset.csv")
 df.head()
```
<img width="1433" height="275" alt="image" src="https://github.com/user-attachments/assets/1beac0e8-3112-4963-90a1-d9246d07e378" />

```python
 x=[1,2,3,4,5]
 y=[3,6,2,7,1]
 sns.lineplot(x=x,y=y)
 plt.title('Line Plot')
```
<img width="881" height="610" alt="image" src="https://github.com/user-attachments/assets/b13f6bff-b834-4eab-9000-011754866b4a" />

```python
 x=[1,2,3,4,5]
 y1=[3,5,2,6,1]
 y2=[1,6,4,3,8]
 y3=[5,2,7,1,4]
 sns.lineplot(x=x,y=y1)
 sns.lineplot(x=x,y=y2)
 sns.lineplot(x=x,y=y3)
 plt.title('Multi Line Plot')
```
<img width="904" height="620" alt="image" src="https://github.com/user-attachments/assets/460b97fe-47f0-44c9-9b96-67bbb3f43488" />

```python
 plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
```
<img width="1381" height="726" alt="image" src="https://github.com/user-attachments/assets/f9e78c7c-64bf-4846-8860-1e53fa1fc95d" />

```python
 sns.scatterplot(x="Age", y="Fare", data=df)
 plt.title('Scatterplot of Age vs Fare')
 plt.show()
```
<img width="765" height="552" alt="image" src="https://github.com/user-attachments/assets/c909a5ae-c9ea-4c13-9e31-01d560d27b53" />

```python
 sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
 plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
 plt.show()
```
<img width="886" height="528" alt="image" src="https://github.com/user-attachments/assets/869b8a66-0038-44d0-ad66-4ce826e9492a" />

```python
sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```
<img width="942" height="493" alt="image" src="https://github.com/user-attachments/assets/abe08ced-e4fd-41e3-b3b3-5c3d5fa8a6ed" />

```python
 sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
 plt.title("Age By Passenger Class")
```
<img width="1361" height="701" alt="image" src="https://github.com/user-attachments/assets/187910b1-fe54-448e-af57-09b7575d165a" />

```python
 sns.violinplot(x="Pclass", y="Fare", data=df)
 plt.title('Violin Plot of Fare by Passenger Class')
 plt.show()
```
<img width="885" height="527" alt="image" src="https://github.com/user-attachments/assets/38634ff9-aad7-4f70-9e09-a69b2bb8e1a6" />

```python
 sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
```
<img width="1083" height="657" alt="image" src="https://github.com/user-attachments/assets/978940c1-cf85-4dac-a47e-14434a7b961f" />

```python
 numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
```
<img width="862" height="638" alt="image" src="https://github.com/user-attachments/assets/0c36f8e4-b593-44bf-a138-9532cb6c4a28" />

# Result:
Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
