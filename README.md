# Bengaluru House Price Project
Here is a description of the project:

Importing Libraries: You started by importing essential libraries such as Pandas, NumPy, and Matplotlib.

Loading Data: You loaded the dataset from a CSV file named "Bengaluru_House_Data.csv" into a Pandas DataFrame (df1).

Exploratory Data Analysis (EDA):
Checked the shape of the DataFrame (13320 rows and 9 columns).
Performed a groupby operation on the 'area_type' column to count occurrences of each area type.

Data Cleaning:
Dropped unnecessary columns ('area_type', 'availability', 'society', 'balcony') from the DataFrame (df2).
Checked for missing values in df2 and dropped rows with missing values.
Extracted the number of bedrooms ('bhk') from the 'size' column and created a new column.

Handling Irregularities:
Identified that the 'total_sqft' column contains a mix of single values and ranges.
Checked for non-numeric values and irregularities in the 'total_sqft' column.

Data Transformation:
Created a function (convert_sqft_to_num) to convert 'total_sqft' values to numeric. The function handles cases where square footage is given as a range.
Applied the conversion function to the 'total_sqft' column in the DataFrame (df4).

Data Exploration:
Checked unique values in the 'bhk' column.
Identified and explored rows where 'bhk' is greater than 20.
