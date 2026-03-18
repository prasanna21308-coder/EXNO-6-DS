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

# Coding:
```
import seaborn as sns
df=sns.load_dataset("tips")
df.head()

df.corr()

df.corr()

sns.heatmap(df.corr())

sns.heatmap(df.corr())
<Axes: >

## Join Plot
sns.jointplot(x='tip',y='total_bill',data=df,kind='hex')
<seaborn.axisgrid.JointGrid at 0x29993779d50>

sns.jointplot(x='tip',y='total_bill',data=df,kind='reg')
<seaborn.axisgrid.JointGrid at 0x2999530f640>

sns.pairplot(df)
<seaborn.axisgrid.PairGrid at 0x29995848e20>

sns.pairplot(df,hue='sex')
<seaborn.axisgrid.PairGrid at 0x299958856c0>

sns.distplot(df['tip'])
sns.distplot(df['tip'])
<Axes: xlabel='tip', ylabel='Density'>
sns.distplot(df['tip'],kde=False,bins=10)
sns.distplot(df['tip'],kde=False,bins=10)
<Axes: xlabel='tip'>
sns.countplot(x='sex', data=df)
<Axes: xlabel='sex', ylabel='count'>
sns.countplot(y='sex',data=df)
<Axes: xlabel='count', ylabel='sex'>
sns.barplot(x='sex',y='total_bill',data=df)
<Axes: xlabel='sex', ylabel='total_bill'>
sns.barplot(x='sex',y='total_bill',data=df)
<Axes: xlabel='sex', ylabel='total_bill'>
|df.head()
sns.boxplot(x='smoker', y='total_bill', data=df)
<Axes: xlabel='smoker', ylabel='total_bill'>
sns.boxplot(x="day", y="total_bill", data=df,palette='rainbow')
<Axes: xlabel='day', ylabel='total_bill'>
sns.boxplot(data=df,orient='v')
<Axes: >
sns.boxplot(x="total_bill", y="day", hue="smoker",data=df)
<Axes: xlabel='total_bill', ylabel='day'>
sns.violinplot(x="total_bill", y="day", data=df,palette='rainbow')
<Axes: xlabel='total_bill', ylabel='day'>
iris = sns.load_dataset('iris')
```

# Result:
 <img width="773" height="574" alt="image" src="https://github.com/user-attachments/assets/c3759703-0da0-4a7b-bf95-6af274d2c6a6" />

<img width="829" height="727" alt="image" src="https://github.com/user-attachments/assets/33dc93f6-59b7-4ca6-853c-3906db803df7" />

