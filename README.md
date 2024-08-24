## Developed by R.Karthikeyan
## Register No:212222240045
## Date:
# Ex.No: 01A PLOT A TIME SERIES DATA
 

# AIM:
To Develop a python program to Plot a time series data of Rainfall rate 
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
data = pd.read_csv("/content/rainfall.csv")

# Convert the 'Date' column to datetime
data['date'] = pd.to_datetime(data['date'])

# Plotting the 'Price' column over time
plt.figure(figsize=(10,6))
plt.plot(data['date'], data['rainfall'], label='rainfall', color='silver')

# Adding title and labels
plt.title('Daily Rainfall')
plt.xlabel('Date')
plt.ylabel('Rainfall rate')

# Displaying the plot
plt.legend()
plt.grid(True)
plt.show()
```

# OUTPUT:
![image](https://github.com/user-attachments/assets/1d35a978-18ac-4469-9100-9ae5521d90ca)






# RESULT:
Thus we have created the python code for plotting the time series of given data.
