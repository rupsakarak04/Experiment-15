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
	​

)/(X
max
	​

−X
min
	​

)
Scales Price between 0 and 1

