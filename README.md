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
