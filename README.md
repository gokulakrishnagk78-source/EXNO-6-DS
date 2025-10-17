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

df = pd.read_csv("titanic_dataset (1).csv")
sns.set(style="whitegrid")

plt.figure(figsize=(8, 6))
sns.countplot(data=df, x="Pclass", hue="Survived", palette="Set2")
plt.title("Survival Count by Passenger Class")
plt.xlabel("Passenger Class")
plt.ylabel("Count")
plt.tight_layout()
plt.show()

plt.figure(figsize=(8, 6))
sns.histplot(data=df, x="Age", hue="Survived", multiple="stack", bins=30, palette="Set1")
plt.title("Age Distribution by Survival")
plt.xlabel("Age")
plt.ylabel("Count")
plt.tight_layout()
plt.show()

plt.figure(figsize=(8, 6))
sns.boxplot(data=df, x="Pclass", y="Fare", palette="Set3")
plt.title("Fare Distribution by Class")
plt.xlabel("Passenger Class")
plt.ylabel("Fare")
plt.tight_layout()
plt.show()

plt.figure(figsize=(8, 6))
sns.countplot(data=df, x="Sex", hue="Survived", palette="coolwarm")
plt.title("Survival Count by Gender")
plt.xlabel("Gender")
plt.ylabel("Count")
plt.tight_layout()
plt.show()

plt.figure(figsize=(8, 6))
sns.scatterplot(data=df, x="Age", y="Fare", hue="Survived", style="Sex", palette="viridis")
plt.title("Age vs Fare Colored by Survival")
plt.xlabel("Age")
plt.ylabel("Fare")
plt.tight_layout()
plt.show()
```
#output:

![Screenshot_17-10-2025_13319_localhost](https://github.com/user-attachments/assets/e260a473-ab6e-4e20-a040-4031858d8d5a)

![Screenshot_17-10-2025_133145_localhost](https://github.com/user-attachments/assets/dc0a5727-0bc0-4203-8a04-dc65e0b4999e)

![Screenshot_17-10-2025_133155_localhost](https://github.com/user-attachments/assets/b2946b3b-9b78-4d82-a637-2128de81bbcd)

![Screenshot_17-10-2025_13328_localhost](https://github.com/user-attachments/assets/b3eea476-e122-4d88-925f-f962a60c0dd9)

![Screenshot_17-10-2025_13319_localhost](https://github.com/user-attachments/assets/de32d67b-b281-43b2-906c-09a8d9c3865f)


# Result:
data visualization process using seaborn library for a sample dataset is performed successfully
 
