# 🌍 Life Expectancy Analysis with EDA
This repository contains an Exploratory Data Analysis (EDA) project using the **Life Expectancy Analysis** dataset, sourced from [Kaggle - Life Expectancy Analysis](https://www.kaggle.com/datasets/nailasrivastava/life-expectancy-analysis/data). The dataset provides a comprehensive overview of health and socio-economic indicators that affect life expectancy across various countries and years.

A quick analysis shows that the dataset covers a time span from **2000 to 2015**. There are **22 columns** representing various indicators related to life expectancy, including **Country**, **Year**, **Status**, **Life expectancy**, **Adult Mortality**, **Infant deaths**, **Alcohol**, **Percentage expenditure**, **Hepatitis B**, **Measles**, **BMI**, **Under-five deaths**, **Polio**, **Total expenditure**, **Diphtheria**, **HIV/AIDS**, **GDP**, **Population**, **Thinness (1–19 years)**, **Thinness (5–9 years)**, **Income composition of resources**, and **Schooling**.


## 📌 Goals
- Examining the statistical summary of each column.
- Identifying missing values and applying appropriate handling techniques.
- Checking for duplicate data entries and removing them as needed.
- Gaining insights into key factors influencing global life expectancy through structured data exploration.


## 🔧 Data Preprocessing Steps
### 1. Reading the Dataset
The dataset was loaded into the Python environment using **pandas** to enable further analysis.

### 2. Data Summary
Used `.info()` to display the structure and content of the dataset, including column names, data types, and non-null counts.

### 3. Checking for Missing Values
Identified missing values in each column and calculated their percentage. Also used statistical summaries to analyze data distribution for numerical and categorical columns.

### 4. Handling Missing Values
Missing data was filled using different strategies based on the data distribution:
- **Mean** (for symmetric distributions): *Life expectancy*, *Total expenditure*, *Income composition of resources*, and *Schooling*.
- **Median** (for skewed distributions): *Adult Mortality*, *Alcohol*, *Hepatitis B*, *BMI*, *Polio*, *Diphtheria*, *GDP*, *Population*, *Thinness 1-19 years*, *Thinness 5-9 years*.

### 5. Handling Duplicate Data
Checked for and removed duplicate entries using `.duplicated().sum()` and `drop_duplicates()` to ensure data quality.


## 🧠 Insights
### 1. Missing Values Identified in Several Columns
Certain columns such as *Hepatitis B*, *BMI*, *GDP*, *Polio*, *Schooling*, etc contain missing values. This indicates that data for some countries may be incomplete or inconsistently reported.

### 2. Data Distribution is Not Always Symmetrical
Based on the statistical summaries, several features like *Adult Mortality*, *Alcohol*, *GDP*, etc show skewed distributions. Understanding this helps in choosing the appropriate method for imputing missing values.

### 3. Missing Value Treatment Based on Distribution
Columns with a normal distribution were filled using the mean, while those with skewed distributions were imputed using the median to preserve data integrity.

### 4. No Duplicate Records Found
A check for duplicate rows revealed none in the dataset, so no further action was required regarding data duplication.


## 🗂️ Document
I also presented my project in the form of a PowerPoint to make it easier to understand. You can view it in the file titled [PPT DSF41DS MONIKA](https://github.com/Monikahung/EDA_Life_Expectancy_Analysis/blob/main/PPT%20DSF41DS%20MONIKA.pdf).

## 📬 Contact
For suggestions, inquiries, or collaboration opportunities, feel free to contact me via [monikahung580@gmail.com](mailto:monikahung580@gmail.com) or connect with me on [linkedin.com/in/monikahung/](https://www.linkedin.com/in/monikahung).

Tags: #Python #EDA #Life_Expectancy_Analysis #Data_Science #Dibimbing #DigitalSkillFair41 #DSF41DS #BootcampDibimbing
