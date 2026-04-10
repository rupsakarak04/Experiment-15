#**EXPERIMENT 15 : Data Normalization & Data Type Conversion**

##*AIM*: **To perform data normalization and data type conversion techniques using Python libraries such as pandas, numpy, and sklearn, and understand how different encoding and scaling methods work on datasets.** 

*THEORY*:

**Data Normalization**

Data normalization is the process of scaling numerical values into a common range without distorting differences in values.

Types used:
Min-Max Normalization → scales values between 0 and 1
Z-score Normalization → standardizes data using mean & standard deviation
Decimal Scaling → scales values by powers of 10

**Data Encoding**

Categorical data must be converted into numerical format for machine learning models.

Methods used:
Label Encoding → assigns unique integer to each category
One-Hot Encoding → creates binary columns for each category
Dummy Encoding → same as one-hot but drops one column to avoid redundancy

1. Creating Dataset: Imports required libraries:

pandas → data handling
numpy → numerical operations

2. Min-Max Normalization:  Rescales the data to a fixed range, usually 0 to 1, by subtracting the minimum and dividing by the range.
Formula: $x_{new} = \frac{x_{old} - x_{min}}{x_{max} - x_{min}}$

Simple Feature Scaling: Divides each value by the maximum value of that column, resulting in a range between 0 and 1.
Formula: $x_{new} = \frac{x_{old}}{x_{max}}$ 

4. Normalizing Multiple Columns: Applies normalization to multiple columns at once.

5. Z-Score Normalization: Z-score Normalization (Standardization): Transforms data to have a mean of 0 and a standard deviation of 1.
Formula: $x_{new} = \frac{x_{old} - \mu}{\sigma}$


6. Decimal Scaling: Divides values by power of 10 and Converts price into scaled-down form

7. Label Encoding: Converts categories into numeric labels

8. Multiple Column Encoding: Encodes multiple categorical columns

9. One Hot Encoding: Creates binary columns for each payment method

10. Dummy Encoding: Drops first column to avoid multicollinearity

## Commands & Functions Used

Function	          Purpose

pd.DataFrame()	  -    Create table

pd.read_csv()	   -   Load dataset

min(), max()	  -    Find range

mean(), std()	  -    Statistical calculations

get_dummies()	  -    One-hot encoding

LabelEncoder()    -    Label encoding

fit_transform()    -   Fit & convert data

*CONCLUSION:*

The experiment successfully demonstrates how raw data can be transformed into a structured and machine-friendly format using normalization and encoding techniques. These preprocessing steps are essential in data analysis and machine learning, as they improve model accuracy, reduce bias, and ensure consistency across datasets.

