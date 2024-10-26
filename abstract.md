Problem Statement: 
Analyzing the Impact of Occupation on Sleep Disorders Based on Lifestyle Factors.

Approach: 
1) Data Cleaning and Preparation: Python (Pandas - For data manipulation, and handling missing values, Numpy - For numerical operations and efficient data handling.)
2) Data Analysis & Visualization: Power BI.
3) (If time permits) Building predictive model: Machine Learning Algorithms.

Data Cleaning & Preparation: 

1. Handling Missing Values: The first step in the data cleaning process is to address null values within the dataset. We utilized the isna() method from the Pandas library to identify missing values column-wise. We applied the fillna() method to impute the null values with the string 'None' to .

3. Checking for Duplicate Data: The presence of duplicate data can skew metrics such as mean, median, and standard deviation, which are crucial for accurately reflecting the true distribution of the data as these are important for detecting outliers. Utilized the duplicated() to detect duplicate values.

4. Analyzing Skewness: Understanding the skewness of the data is essential for selecting appropriate statistical methods. We calculated the skewness of relevant data columns using the skew() method. The skewness score was found to be very close to 0, indicating that the data is approximately symmetric. Therefore, using the mean as the preferred statistical method for further analysis for outlier detection is appropriate.

5. Handling Outliers: We employed the Z-score method to detect them. According to this method, a data point is classified as an outlier if its Z-score falls outside the range of (-3) to (+3). Our analysis indicated that both the 'Age' and 'Number_of_Virtual_Meetings' columns do not exhibit significant bias.

Key performance Indicators:
1) Impact on mental health based on the mode of work.
2) Work-life balance varies significantly based on the hours worked and virtual meetings attended 
3) Visualization of Mental Health Conditions based on Region.
4) What is the relation of stress levels on quality of sleep and productivity changes?
5) How has remote work impacted productivity across different job roles and industries?
6) Are employees experiencing higher levels of social isolation more likely to report lower satisfaction with remote work?
7) What is the impact of physical activity on the mental health condition of remote workers?

