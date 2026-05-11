# Police_data_Analysis-using-Python_Pandas


**📌 Project Overview**

This project performs Exploratory Data Analysis (EDA) on a police dataset using Python and Pandas.
The dataset contains information about traffic stops, driver details, violations, searches, and stop durations.

The notebook demonstrates how to clean, analyze, filter, and extract useful insights from the dataset using various Pandas operations.

**📂 Dataset Description**

The dataset includes the following features:

Driver Gender
Driver Age
Violation Type
Search Conducted
Stop Duration
Country/State Information
Speeding Records
Drug & Alcohol Related Stops

It is a structured dataset used for analyzing police traffic stop records.

**🛠️ Technologies Used**
Python 🐍
Pandas 📊
Jupyter Notebook

**🔍 Key Concepts Covered**
📊 Data Exploration
Viewing dataset using head()
Checking dataset shape using shape
Viewing column names
Dataset summary using info()
Detecting null values using isnull().sum()

**🧹 Data Cleaning**
Handling missing values using fillna()
Converting string values to numeric format
Removing unwanted rows using filtering
Fixing datatype issues

**Example:**

police.isnull().sum()
police.fillna(0)

**📈 Data Analysis Techniques**
✔️ Value Counts-->Finding unique values and their occurrences.

  syntax:police['driver_gender'].value_counts()
  
✔️ Filtering Data-->Filtering records based on conditions.

  syntax:police[police['violation'] == 'Speeding']
  
✔️ GroupBy Operations-->Grouping records for better analysis.

  syntax:police.groupby('driver_gender')['search_conducted'].sum()
  
✔️ Statistical Operations-->Performing statistical calculations.

 syntax: police['driver_age'].mean()
         police['driver_age'].max()
         police['driver_age'].min()

📊 Sample Questions Solved

**Q1. Which gender was stopped more often for speeding?**

Used filtering and value_counts() to analyze speeding violations.

**Q2. How many searches were conducted for each gender?**

Used groupby() and sum() for analysis.

**Q3. What is the average driver age?**

Used statistical functions like mean().

**Q4. How to identify missing values?**

Used isnull().sum().

**Q5. How to clean null values?**

Used fillna() method.

📁 Project Structure
├── Police Data Analysis.ipynb
├── police_data.csv
├── README.md

**📌 Key Insights**
Male drivers were stopped more frequently for speeding.
GroupBy operations help in comparing records efficiently.
Missing values can be handled easily using Pandas.
Filtering makes data analysis more accurate.
Pandas provides powerful functions for real-world dataset analysis.

**🎯 Conclusion**

This project showcases how Pandas can be used for real-world police data analysis by applying data cleaning, filtering, grouping, and statistical techniques. It helps in understanding traffic stop patterns and extracting meaningful insights from the dataset efficiently.
