# Excel_Project-Data_Analytics  
## Excel Salary Dashboard  
![1_Salary_Dashboard_Final_Dashboard](https://github.com/user-attachments/assets/a48f2ee0-c31f-4fc5-93a2-81c1e54b1fda)  
### Introduction  
This data jobs salary dashboard was created to help job seekers investigate salaries for their desired jobs and ensure they are being adequately compensated.  
### Dashboard File  
My final dashboard is [Salary_Dashboard](Project_1-Dashboard).  
### Excel Skills Used  
I utilized the following Excel skills for analysis:  

- Charts
- Formulas and Functions
- Data Validation

## Dashboard Build  
### Charts
**Data Science Job Salaries - Bar Chart**  

![Data_job_salaries_bar_chart](https://github.com/user-attachments/assets/33a8ac4b-accf-4a2d-b6aa-8b2ad98ae7d3)  
- **Excel Features:** Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- **Insights Gained:** This enables quick identification of salary trends, noting that Senior roles and Engineers are higher- 
                       paying than Analyst roles.

**Country Median Salaries - Map Chart**   

![1_Salary_Dashboard_Country_Map](https://github.com/user-attachments/assets/b760b223-fb57-483e-8f38-fe0b9c5fbefc)  

- **Excel Features:** Utilized Excel's map chart feature to plot median salaries globally.
- **Insights Gained:** Enables quick grasp of global salary disparities and highlights high/low salary regions.

### Formulas and Functions  

**Median Salary by Job Titles**  

![median_salaries](https://github.com/user-attachments/assets/5aae826d-2f0c-4198-8345-e1edb5572138)  

- **Multi-Criteria Filtering:** Checks job title, country, schedule type, and excludes blank salaries.  
- **Array Formula:** Utilizes MEDIAN() funtion with nested IF() statement to analyze an array.
- **Tailored Insights:** Provides specific salary information for job titles, regions and schedule types.
- **Formula Purpose:** This formula populates the table below, returning the median salary based on job title, country and type specified.

**Background Table**  
![salary_table](https://github.com/user-attachments/assets/1b5ac614-34a8-4a45-b9bc-c5afc33b7013)  

**Dashboard Implementation**  
![title implementation](https://github.com/user-attachments/assets/d829979a-350c-4ba0-9673-aa40d6deb63f)  

### Data Validation  

**Filtered List**  

- **Enhanced Data Validation:** Implementing the filtered list as a data validation rule under the Job Title, Country and Type option in Data tab ensures:
  1. User input is restricted to predefined, validated schedule types.  
  2. Incorrect or inconsistent entries are prevented.  
  3. Overall usability of the dashboard is enhanced.
 
![1_Salary_Dashboard_Data_Validation](https://github.com/user-attachments/assets/819490bc-1a79-4a56-9245-8330111d8d84)  

### Conclusion  

This dashboard was created to showcase insights into salary trends across various data-related job titles. This dashboard allows users to make informed decisions about their career paths, Exploring the functionalities to understand how location and job type influences salaries.  

# Project 2 Analysis  
## Introduction  
As a current job seeker curious about data and the data science job market, I’ve noticed a lack of data-driven insights into the most optimal roles and in-demand skills. To make an informed career decision, I’m analyzing what top employers seek and which skills lead to higher pay.  
## Questions to Analyze  
To understand the data science job market, I asked the following:  
1. Do more skills get you better pay?
2. What's the salary for data jobs in different regions?
3. What are the top skills of data professionals?
4. What's the pay for the top 10 skills?
## Excel Skills Used  
I utilized following Excel skills for analysis:  
- Pivot Tables
- Pivot Charts
- DAX (Data Analysis Expressions)
- Power Query
- Power Pivot
## 1. Do more skills get you better pay?  
### Skill: Power Query (ETL)  
**i) Extract**  
- First I used Power Query to extract the original data and create two queries:  
  - First one with all the data job information.
  - The second listing the skills for each job id.

**ii) Transform**  
- Then, I transformed each query by changing coloumn types, removing unnecessary coloumns, cleaning text to eliminate specific words and trimming excess whitespace.

  - **data job salary**
  
  ![Screenshot 2025-02-08 152220](https://github.com/user-attachments/assets/124e4324-aa83-4650-b250-de040a86b474)

  - **data job skills**

    ![Screenshot 2025-02-08 152908](https://github.com/user-attachments/assets/8ba4ea45-f2d7-4394-a667-17bb6fb1fab6)

**iii) Load**  
- Finally, I loaded both transformed queries into the workbook, setting the foundation for my subsequent analysis.

  - **data job salary**  

    ![Screenshot (427)](https://github.com/user-attachments/assets/db93c104-9062-4caa-8f84-0951b165e664)

  - **data job skills**

    ![Screenshot (428)](https://github.com/user-attachments/assets/57ae8648-7f0c-43ef-b96d-77de128d3d0c)

### Analysis  
**Insights**  
- There is a positive correlation between the number of skills requested in job postings and the median salary, particularly in roles like Senior Data Engineer and Data Scientist.
- Roles that require fewer skills, like Business Analyst, tend to offer lower salaries, suggesting that more specialized skill sets command higher market value.

  ![Screenshot 2025-02-08 153936](https://github.com/user-attachments/assets/794de0aa-da29-4bcc-9a52-d29ebd2c9e7e)

**Conclusion**  
- This trend emphasizes the value of aquiring multiple relevant skills, particularly for individuals aiming for higher-paying roles.
## 2. What's the salary for data jobs in different regions?  
### Skills: PivotTables & DAX  
**Pivot Table**  
- I created a PivotTable using Data Model I created with Power Pivot.
- I moved the job_titlr_short to the rows area and slary_year_avg into the values area.
- Then I added new measure to calculate the median salary for United States jobs.
  


  



  
  

    
  

















