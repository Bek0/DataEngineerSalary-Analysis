# Salary Data Analysis Project

## Overview

This project analyzes a dataset of salaries to provide insights into various factors affecting salaries, such as job title, location, experience level, and company size. The project includes steps for data cleaning, preprocessing, and visualization of trends in the dataset.

## Dataset

The dataset used in this analysis contains information on salaries across different job titles, company locations, employee residences, experience levels, and more. The key steps in this project include loading the data, cleaning and preprocessing it, and performing visual analysis to extract meaningful insights.

## Project Structure

1. **Loading the Data**
   - The dataset is loaded into a Pandas DataFrame for further analysis.
   - Basic exploratory analysis, including checking data types, shape, and descriptive statistics.

2. **Data Cleaning and Preprocessing**
   - **Handling Missing Values:** Checked for missing data and counted missing values for each column.
   - **Removing Duplicates:** Duplicated rows are identified and removed.
   - **Filtering Data:** The dataset is filtered to include only records where the `work_year` is greater than 2020.
   - **Column Removal:** Dropped columns that are not needed for this analysis, such as `salary_currency` and `salary`.
   - **Value Replacement:**
     - The `remote_ratio` column is updated with meaningful labels:
       - 0 → "on site"
       - 50 → "hybrid"
       - 100 → "remote"
     - Job titles are standardized (e.g., "Machine Learning Engineer" is replaced with "ML Engineer").
     - The company and employee locations are updated by replacing "IL" with "PS" to maintain consistency.

3. **Data Visualization**
   - The analysis focuses on various factors affecting salary, providing insights into trends, distributions, and relationships between different features.

## Key Analysis Questions

1. **How has the average salary changed over the years?**
2. **What is the average salary for each experience level, and how do they rank?**
3. **How does the average salary vary across different employment types?**
4. **How does the average salary vary across different company sizes?**
5. **How does the average salary change over the years for companies of different sizes?**
6. **How does the average salary change over the years for companies based on their remote work ratio?**
7. **Which are the top 5 countries with the most employees?**
8. **How does the average salary vary across the top 10 employee residences based on employee count?**
9. **How do the average salaries compare across the top 10 company locations by employee count?**
10. **What is the distribution of remote work ratios within each company size category?**
11. **Which are the top 5 countries with the most employees in large companies?**
12. **Which are the top 5 countries with the most experienced employees?**
13. **What are the top 10 salaries in the dataset?**
14. **What are the top 5 and bottom 5 average salaries by job title among all jobs?**
15. **What are the top 10 most prevalent job titles among employees?**
16. **How does the average salary change over the years for the top 5 most prevalent job titles?**
17. **How does the average salary change over the years for the top 5 most prevalent jobs?**
18. **What are the top 5 most prevalent job titles each year, presented as a percentage of total jobs for that year?**
19. **What are the top 5 most prevalent job titles within small (S), medium (M), and large (L) companies, presented as a percentage of total job titles in each company size category?**
20. **What are the top 5 jobs with the highest salary increase over the years and the top 5 jobs with the lowest salary decrease over the years?**
21. **What are the top 5 job titles or fields with the highest increase and decrease in employment count over the years?**

## Libraries Used

- **Pandas**: For data loading, manipulation, and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For basic data visualization.
- **Seaborn**: For advanced data visualization and aesthetics.
- **Warnings**: To manage warnings during the analysis process.

## Data Cleaning and Transformation

- **Dropped Duplicates**: Identified and removed all duplicate rows from the dataset.
- **Filtered Rows**: Included only rows where `work_year` is greater than 2020 for more relevant analysis.
- **Replaced Values**: Adjusted various columns for consistency, such as `remote_ratio`, `job_title`, `company_location`, and `employee_residence`.

## Conclusion

This project provided insights into how salary is affected by various factors like experience, job title, location, and company size. Visualizations helped uncover trends and patterns that can be useful for understanding the dynamics of salaries across different sectors.

---

