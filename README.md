# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 07-03-2025
### Name: Jeshwanth Kumar P

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```p
import pandas as pd
import matplotlib.pyplot as plt

df=pd.read_csv('data.csv')
df.shape
df1=df.head(100)
df1
```
![image](https://github.com/user-attachments/assets/6cbbfb9b-fa6c-4345-a5e1-d128b7594e46)
```p
df.info()
```
![image](https://github.com/user-attachments/assets/39591344-f183-4586-aba4-b22c6a076086)
```p
df.describe()
```
![image](https://github.com/user-attachments/assets/58e0c1c7-aae7-4615-a9df-a266664f8f7d)

```p
x=df1['yr_built']
y=df1['price']

plt.figure(figsize=(15,8))
plt.bar(x,y)
plt.grid(True)
plt.title('Price vs Year Built')
plt.xlabel('Year Built')
plt.ylabel('Price')
plt.show()
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/e6fc9ec1-e8f2-47ec-9bea-e873e11e7ad9)
# RESULT:
Thus we have created the python code for plotting the time series of given data.
