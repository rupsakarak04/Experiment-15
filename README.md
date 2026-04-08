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

2. Min-Max Normalization: Formula:

(
𝑋
−
𝑋
𝑚
𝑖
𝑛
)
/
(
𝑋
𝑚
𝑎
𝑥
−
𝑋
𝑚
𝑖
𝑛
)
(X−X
min
)/(X
max
−X
min
)

Scales Price between 0 and 1

3. Normalizing Multiple Columns: Applies normalization to multiple columns at once

4. Z-Score Normalization: Formula:

(
𝑋
−
𝜇
)
/
𝜎
(X−μ)/σ

Centers data around mean = 0

5. Decimal Scaling: Divides values by power of 10 and Converts price into scaled-down form

6. Label Encoding: Converts categories into numeric labels

7. Multiple Column Encoding: Encodes multiple categorical columns

8. One Hot Encoding: Creates binary columns for each payment method

9. Dummy Encoding: Drops first column to avoid multicollinearity

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

