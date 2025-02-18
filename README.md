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

![Screenshot 2025-02-18 223623](https://github.com/user-attachments/assets/389f810e-3de0-462d-a6ef-d5404324b386)

- **Excel Features:** Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- **Insights Gained:** This enables quick identification of salary trends, noting that Senior roles and Engineers are higher paying than Analyst roles.

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
![Screenshot 2025-02-18 223633](https://github.com/user-attachments/assets/3144820e-d9b1-40a3-b88e-b43158b15be5)  


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
 
  ![Screenshot 2025-02-08 162252](https://github.com/user-attachments/assets/6717638f-f4c1-44df-998e-b9eb70434177)

**DAX**  
- I used DAX to calculate median year salary.

  ![Screenshot 2025-02-08 162454](https://github.com/user-attachments/assets/a0c93404-d5f0-487d-a38d-9142fc89f2f5)

## Analysis  
**Insights**  
- Job roles like Senior Data Engineer and Data Scientist command higher median salaries both in the US and internationally, showcasing the global demand for high-level data expertise.  
- The salary disparity between US and Non-US roles is particularly notable in high-tech jobs, which might be influenced by the concetraction of tech industries in the US.

  ![Screenshot 2025-02-08 165335](https://github.com/user-attachments/assets/85e64e34-5651-49ed-890f-f4d1c05cfa80)

**Conclusion**  
- These salary insights are important for planning and salary negotiations, helping professionals and companies align their offers with market standards while considering geographical variations.

## 3. What are the top skills of data professionals?  
### Skill: Power Pivot  
**Power Pivot**  
- I created a data model by integrating the (data job salary) and (data jo skills) tables into one model.  
- Since I had already cleaned the data using Power Query; Power Pivot created a relationship between these two tables.
### Data Model  
- I created a relationship between my two table using the job id coloumn.
  
  ![Screenshot 2025-02-08 170311](https://github.com/user-attachments/assets/e4054dac-e227-4998-9853-71319ab26352)

**Power Pivot Menu**  
- The Power Pivot menu was used to refine my data model and makes it easy to create measures.

  ![Screenshot 2025-02-08 170636](https://github.com/user-attachments/assets/3e6f6b36-e903-4365-95d2-075253c4773b)

## Analysis  
**Insights**  
- SQL, Excel and Python dominates as top skills for data analyst role in India.
- Emerging technologies like AWS and Azure also show significant presence, underlinining the industry's shift toward cloud services and big data technologies.  
  
![Screenshot 2025-02-08 171553](https://github.com/user-attachments/assets/40cef6d1-00ca-4cad-9b9c-2430a4ff7e60)  

**Conclusion**  
- Understanding prevelant skills in the industry not only helps professionals stay competitive but also guides training and educational programs to focus on tje most impactful technologoes.

## 4. What's the pay of the top 10 skills?  
### Skill: Advanced Charts (Pivot Chart)  
**PivotChart**  
- I created a combo PivotChart to plot median salary and skill liklihood(%) from my pivotTable.
  - Primary Axis: Median Salary (as a clustered coloumn)
  - Secindary Axis: Skill Likelihood (asa line with markers)
- To customize the chart, I added a title axis title, removed the lines (skill liklihood), and changed the markers to diamonds.

## Analysis  
**Insights**  
- Higher median salaries are associated with skills like Python, Oracle and SQL, suggesting their critical role in high-paying tech jobs.
- Skills like PowerPoint and Word have the lowest median salaries and liklihood, indicating less specialization and demand in high-salary sectors.

  ![Screenshot 2025-02-08 172939](https://github.com/user-attachments/assets/eaadbacd-9e1b-4447-aa20-c7c0f76d4b2b)

**Conclusion**  
- This Chart highlights the importance of investing time in learning high-value skills like Python and SQL, which are evidently tied to higher paying roles, especially for those looking to maximize their salary in the tech industry.

## Final Conclusion  
As a data enthusiast and a job seeker, I embarked on this Excel-based project to uncover valuable insights about the data science job market. Using a real-world job postings dataset, I analyzed job titles, salaries, locations and essential skills. By leveraging Excel features like Power Query, PivotTables, DAX and Charts, I discovered key correlations between multiple skills and higher salaries, particularly in Python, SQL and cloud technologies.  
I hope this project provides an overview of the skills needed for higher-paying roles.  

**PS:** In the salary dashboard you may find for some permutation of job_title, country and job_type that a few job titles or job type data fields are empty in the bar chart I used. This is happening because for a particular country there are no job openings available for a particular job role or job type. And when you switch between different job roles or country or job type you may notice that the bar charts does not remain sorted.  

This can also be fixed by using some dynamic array functions like FILTER() and SORT() functions available in Excel365 or Excel 2021 or newer versions but I unfortunately don't have acces to these dynamic array functins, So I couldn't use them in my project.  

I made this project by following along a course available on youtube which goes by "Excel_for_Data_Analytics" uploaded by "Luke Barrouse" on his youtube channel [LukeBarrouse](https://youtu.be/pCJ15nGFgVg?feature=shared) and the dataset used for this project is a real world data.





