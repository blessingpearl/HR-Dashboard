# HR ANALYTICS BUSINESS REPORT
# TABLE OF CONTENT
## Project Overview
## Tools And Technology
## Datasets overview
## Data Cleaning And Power BI Dashboard
## Key Insights
## Recommendations
## Future Works 
## Repository Structure
# Project Overview 
This report analyzes the organization's workforce using an HR Power BI dashboard. The dashboard focuses on employee numbers, termination, salary, job satisfaction, work-life balance, education, gender, and workforce trends.
# Tools And Technology
power bi
# Datasets overview
Attrition	Business Travel	CF_age band	CF_attrition label	Department	Education Field	emp no	Employee Number	Gender	Job Role	Marital Status	Over Time	Over18	Training Times Last Year	-2	0	Age	CF_current Employee	Daily Rate	Distance From Home	Education	Employee Count	Environment Satisfaction	Hourly Rate	Job Involvement	Job Level	Job Satisfaction	Monthly Income	Monthly Rate	Num Companies Worked	Percent Salary Hike	Performance Rating	Relationship Satisfaction	Standard Hours	Stock Option Level	Total Working Years	Work Life Balance	Years At Company	Years In Current Role	Years Since Last Promotion	Years With Curr Manager
<img width="5271" height="22" alt="image" src="https://github.com/user-attachments/assets/0bea7c7e-4056-4290-8860-1338f2391bd1" />
# Data Cleaning And Power BI Dashboard
Extract, transform and Load in Power BI
Changed data type
Removed unwanted columns
Created a calender table using query editor for the purpose of creating days of week and name of days before loading


Data Modeling
Employee Table - Fact Table
Calender Table - dimension Table
Relationship connection between both is the Order Date column Employee table and Date column on the calender table

DAX measure:
current employee = CALCULATE(COUNTROWS(Employee), FILTER(Employee, Employee[Attrition] = "No" ))
total employee = COUNT(Employee[ID_employe])

Data visualization
Visuals used are; card, clustered bar chart and line chart

# Key Insights
