
#EXP-10-Datascience-process
#AIM :
To Perform Data Science Process on a complex dataset and save the data to a file.

#ALGORITHM :
#STEP 1:
Read the given Data

#STEP 2:
Clean the Data Set using Data Cleaning Process

#STEP 3:
Apply Feature Generation/Feature Selection Techniques on the data set

#STEP 4:
Apply EDA /Data visualization techniques to all the features of the data set

# PROGRAM
```
DEVELEOPED BY:SWETHA P
REGISTER NUMBER:212222100053
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
data = pd.read_csv("Salary_Data.csv")
print(data.head())
print(data.info())
print(data.describe())
sns.histplot(data['Salary'], kde=True)
plt.xlabel('Salary')
plt.ylabel('Count')
plt.title('Distribution of Salaries')
plt.show()
sns.scatterplot(data=data, x='Age', y='Salary')
plt.xlabel('Age')
plt.ylabel('Salary')
plt.title('Salary vs. Age')
plt.show()
plt.figure(figsize=(8, 6))
plt.hist(data['Salary'], bins=20, edgecolor='black')
plt.xlabel('Salary')
plt.ylabel('Count')
plt.title('Distribution of Salaries')
plt.show()
plt.figure(figsize=(8, 6))
plt.boxplot(data['Salary'], vert=False)
plt.xlabel('Salary')
plt.title('Box Plot of Salaries')
plt.show()
corr_matrix = data.corr()
plt.figure(figsize=(10, 8))
sns.heatmap(corr_matrix, annot=True, cmap="coolwarm")
plt.title("Correlation Heatmap for Salary Dataset")
plt.show()
plt.figure(figsize=(8, 6))
sns.violinplot(data=data, y='Salary')
plt.ylabel('Salary')
plt.title('Distribution of Salaries')
plt.show()
```

# OUTPUT
![Screenshot 2023-06-05 200110](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/380454ed-bbb1-447c-b545-cd02d08e53fa)
![Screenshot 2023-06-05 203245](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/0903eab5-ddd3-4e00-bdea-ad2543f23eae)
![Screenshot 2023-06-05 203307](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/29b2223f-1f57-4f55-96c4-2a9aa476c2e5)
![Screenshot 2023-06-05 203345](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/07a125eb-96a0-4219-815d-d6894fda5931)
![Screenshot 2023-06-05 203415](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/be32ba6d-9b86-4792-be00-bc0f605af9fe)
![Screenshot 2023-06-05 203439](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/46ae1176-5976-4e51-ac38-cb7c362d9340)
![Screenshot 2023-06-05 203508](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/4442025e-d99b-4cf3-897d-2e4709c4e465)
![Screenshot 2023-06-05 203523](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/e87039b4-a368-4c91-bae1-d32d3797d44e)
![Screenshot 2023-06-05 203541](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/fa7db6c7-02bd-427d-8636-5bc45b835c66)
![Screenshot 2023-06-05 203559](https://github.com/swetha1510/eEX-10-DATASCIENCE/assets/120623583/b9e32eb9-d2f3-4cef-820c-64d8baab2522)

RESULT
Thus, we have read the given data and Performed Data Science Process on a complex dataset



