Problem Statement: 
Analyzing the Impact of Occupation on Sleep Disorders Based on Lifestyle Factors. 

Dataset:The dataset includes details such as gender, age, occupation, sleep duration, quality of sleep, physical activity level, stress levels, BMI category, blood pressure, heart rate, daily steps, and the presence or absence of sleep disorders.

Approach: 
1) Data Cleaning and Preparation: Python (Pandas - For data manipulation, and handling missing values, Numpy - For numerical operations and efficient data handling.)
2) Data Analysis & Visualization: Tableau.
3) (If time permits) Building predictive model: Machine Learning Algorithms.

Data Cleaning & Preparation: 

1. Handling Missing Values: The first step in the data cleaning process is to address null values within the dataset. We utilized the isna() method from the Pandas library to identify missing values column-wise. We applied the fillna() method to impute the null values with the string 'None' to .

3. Checking for Duplicate Data: The presence of duplicate data can skew metrics such as mean, median, and standard deviation, which are crucial for accurately reflecting the true distribution of the data as these are important for detecting outliers. Utilized the duplicated() to detect duplicate values.

4. Analyzing Skewness: Understanding the skewness of the data is essential for selecting appropriate statistical methods. We calculated the skewness of relevant data columns using the skew() method. The skewness score was found to be very close to 0, indicating that the data is approximately symmetric. Therefore, using the mean as the preferred statistical method for further analysis for outlier detection is appropriate.

5. Handling Outliers: We employed the Z-score method to detect them. According to this method, a data point is classified as an outlier if its Z-score falls outside the range of (-3) to (+3). Our analysis indicated that both the 'Age' and 'Number_of_Virtual_Meetings' columns do not exhibit significant bias.


