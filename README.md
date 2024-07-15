# Sea-Level-Predictor-
This project uses Python to analyze historical sea level data and predict future trends up to 2050 using linear regression.

# sea_level_predictor.py

import pandas as pd
import matplotlib.pyplot as plt
from scipy.stats import linregress
import numpy as np

# Step 1: Importing Data
df = pd.read_csv('epa-sea-level.csv')

# Step 2: Handling Missing Values
df.dropna(inplace=True)  # Drop rows with missing values if any

# Step 3: Convert columns to numeric if needed
df['Year'] = pd.to_numeric(df['Year'])
df['CSIRO Adjusted Sea Level'] = pd.to_numeric(df['CSIRO Adjusted Sea Level'])

# Step 4: Creating a Scatter Plot
plt.figure(figsize=(10, 6))
plt.scatter(df['Year'], df['CSIRO Adjusted Sea Level'], color='blue', label='Data')

# Step 5: Fitting a Linear Regression
slope, intercept, r_value, p_value, std_err = linregress(df['Year'], df['CSIRO Adjusted Sea Level'])

# Predicting sea level rise till 2050
plt.plot([1880, 2050], [intercept + slope*1880, intercept + slope*2050], color='red', linestyle='-', linewidth=2, label='Linear Regression (1880-2014)')

# Step 6: Labeling and Saving
plt.xlabel('Year')
plt.ylabel('Sea Level (inches)')
plt.title('Rise in Sea Level')
plt.legend()

# Save the plot as an image
plt.savefig('sea_level_plot.png')

# Display the plot
plt.show()
# sea_level_predictor.py

import pandas as pd
import matplotlib.pyplot as plt
from scipy.stats import linregress
import numpy as np

# Step 1: Importing Data
df = pd.read_csv('epa-sea-level.csv')

# Step 2: Handling Missing Values
df.dropna(inplace=True)  # Drop rows with missing values if any

# Step 3: Convert columns to numeric if needed
df['Year'] = pd.to_numeric(df['Year'])
df['CSIRO Adjusted Sea Level'] = pd.to_numeric(df['CSIRO Adjusted Sea Level'])

# Step 4: Creating a Scatter Plot
plt.figure(figsize=(10, 6))
plt.scatter(df['Year'], df['CSIRO Adjusted Sea Level'], color='blue', label='Data')

# Step 5: Fitting a Linear Regression
slope, intercept, r_value, p_value, std_err = linregress(df['Year'], df['CSIRO Adjusted Sea Level'])

# Predicting sea level rise till 2050
plt.plot([1880, 2050], [intercept + slope*1880, intercept + slope*2050], color='red', linestyle='-', linewidth=2, label='Linear Regression (1880-2014)')

# Step 6: Labeling and Saving
plt.xlabel('Year')
plt.ylabel('Sea Level (inches)')
plt.title('Rise in Sea Level')
plt.legend()

# Save the plot as an image
plt.savefig('sea_level_plot.png')

# Display the plot
plt.show()
# sea_level_predictor.py

import pandas as pd
import matplotlib.pyplot as plt
from scipy.stats import linregress
import numpy as np

# Step 1: Importing Data
df = pd.read_csv('epa-sea-level.csv')

# Step 2: Handling Missing Values
df.dropna(inplace=True)  # Drop rows with missing values if any

# Step 3: Convert columns to numeric if needed
df['Year'] = pd.to_numeric(df['Year'])
df['CSIRO Adjusted Sea Level'] = pd.to_numeric(df['CSIRO Adjusted Sea Level'])

# Step 4: Creating a Scatter Plot
plt.figure(figsize=(10, 6))
plt.scatter(df['Year'], df['CSIRO Adjusted Sea Level'], color='blue', label='Data')

# Step 5: Fitting a Linear Regression
slope, intercept, r_value, p_value, std_err = linregress(df['Year'], df['CSIRO Adjusted Sea Level'])

# Predicting sea level rise till 2050
plt.plot([1880, 2050], [intercept + slope*1880, intercept + slope*2050], color='red', linestyle='-', linewidth=2, label='Linear Regression (1880-2014)')

# Step 6: Labeling and Saving
plt.xlabel('Year')
plt.ylabel('Sea Level (inches)')
plt.title('Rise in Sea Level')
plt.legend()

# Save the plot as an image
plt.savefig('sea_level_plot.png')

# Display the plot
plt.show()
# sea_level_predictor.py

import pandas as pd
import matplotlib.pyplot as plt
from scipy.stats import linregress
import numpy as np

# Step 1: Importing Data
df = pd.read_csv('epa-sea-level.csv')

# Step 2: Handling Missing Values
df.dropna(inplace=True)  # Drop rows with missing values if any

# Step 3: Convert columns to numeric if needed
df['Year'] = pd.to_numeric(df['Year'])
df['CSIRO Adjusted Sea Level'] = pd.to_numeric(df['CSIRO Adjusted Sea Level'])

# Step 4: Creating a Scatter Plot
plt.figure(figsize=(10, 6))
plt.scatter(df['Year'], df['CSIRO Adjusted Sea Level'], color='blue', label='Data')

# Step 5: Fitting a Linear Regression
slope, intercept, r_value, p_value, std_err = linregress(df['Year'], df['CSIRO Adjusted Sea Level'])

# Predicting sea level rise till 2050
plt.plot([1880, 2050], [intercept + slope*1880, intercept + slope*2050], color='red', linestyle='-', linewidth=2, label='Linear Regression (1880-2014)')

# Step 6: Labeling and Saving
plt.xlabel('Year')
plt.ylabel('Sea Level (inches)')
plt.title('Rise in Sea Level')
plt.legend()

# Save the plot as an image
plt.savefig('sea_level_plot.png')

# Display the plot
plt.show()
![image](https://github.com/user-attachments/assets/ca820a7c-8e7e-4248-8540-7675a398ca82)
