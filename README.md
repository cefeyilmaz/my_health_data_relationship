# What is this project?
This is a data science project investigating the relationship between my Headphone Audio Exposure and Step Count values.

# Data I Gathered:
* Exported a xml file from Apple Health app.

# How To Use:
1) Convert Apple health xml file to csv file.
2) Delete unwanted data with certain operations step by step
3) Use lastly modified csv file to train/test models.

# 1)Converting XML to CSV
* I used a pre designed script made by Jason Meno for converting
* Here is Github repository of that script: https://github.com/jameno/Simple-Apple-Health-XML-to-CSV

# 2) Data Preperation
* Step by step data preperation:
1) Filter data by selecting only 'HeadphoneAudioExposure' and 'StepCount' types. Then choose only selected columns.
2) Sum all values in one day and convert date type to day.
3) Filter data one more time with date range from '2022.01.01' to '2023.12.31'.
4) Correct numbers with error like '26.764.660.000.000.000'.
5) Delete rows if date is not common for two types.

# 3) Prepare and split the data into train and test
* Used test size = 0.2

# 4) Explore and visualize data
* Print some information about data.
* Create some graphs to look for a relationship.

# 5) Machine Learning Models
* XGBoost Model
* Random Forest Model

# 6) Comparison
* Compare two models with visual data
* Compare two models with numerical data  
