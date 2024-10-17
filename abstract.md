Problem Statement: 
Empowering Corporate Wellness: Analyzing the Impact of Job Roles and Work Locations on Mental Health
Following the COVID-19 pandemic, remote work rapidly became the new norm, significantly transforming the work culture, particularly within the tech industry. In this project, we aim to visually represent the collected data to gain insights into the mental health conditions of employees working in various settings across the globe. This dashboard will help companies from diverse industries identify which work environments are most effective in maximizing productivity while prioritizing employees’ mental well-being.

Approach: 
1) Data Cleaning and Preparation: Python (Pandas - For data manipulation, and handling missing values, Numpy - For numerical operations and efficient data handling.)
2) Data Analysis & Visualization: Power BI.
3) (If time permits) Building predictive model: Machine Learning Algorithms.

Data Cleaning & Preparation: 

1. Handling Missing Values: The first step in the data cleaning process is to address null values within the dataset. We utilized the isna() method from the Pandas library to identify missing values column-wise. Our analysis revealed that the columns 'Mental_Health_Condition' and 'Physical_Activity' contained over 1,100 and 1,600 null values, respectively. As the dataset consists of only 5,000 rows, removing rows with null values would result in significant data loss. Therefore, we applied the fillna() method to impute the null values with the string 'Not Reported'.

3. Checking for Duplicate Data: The presence of duplicate data can skew metrics such as mean, median, and standard deviation, which are crucial for accurately reflecting the true distribution of the data as these are important for detecting outliers. Utilized the duplicated() to detect duplicate values.

4. Analyzing Skewness: Understanding the skewness of the data is essential for selecting appropriate statistical methods. We calculated the skewness of relevant data columns using the skew() method. The skewness score was found to be very close to 0, indicating that the data is approximately symmetric. Therefore, using the mean as the preferred statistical method for further analysis for outlier detection is appropriate.

5. Handling Outliers: In our dataset, two numerical columns 'Age' and 'Number_of_Virtual_Meetings' were identified as potentially containing outliers. We employed the Z-score method to detect them. According to this method, a data point is classified as an outlier if its Z-score falls outside the range of (-3) to (+3). Our analysis indicated that both the 'Age' and 'Number_of_Virtual_Meetings' columns do not exhibit significant bias.

Key performance Indicators:
1) Impact on mental health based on the mode of work.
2) Work-life balance varies significantly based on the hours worked and virtual meetings attended 
3) Visualization of Mental Health Conditions based on Region.
4) What is the relation of stress levels on quality of sleep and productivity changes?
5) How has remote work impacted productivity across different job roles and industries?
6) Are employees experiencing higher levels of social isolation more likely to report lower satisfaction with remote work?
7) What is the impact of physical activity on the mental health condition of remote workers?

