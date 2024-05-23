# HR- Employee Attrition Project

### Report Link :https://drive.google.com/file/d/1_8PW1DURVZl1G58n8IyTEh-0W4qXmQwd/view?usp=sharing

## Problem Statement

The aim of this project is to develop a comprehensive and dynamic dashboard using Power BI to track, analyze, and visualize employee attrition and satisfaction across various departments and demographic groups within the company. By providing detailed insights into current attrition rates, job satisfaction levels, and demographic profiles, this project seeks to enhance employee retention strategies, improve workforce satisfaction, and foster a positive organizational culture. The analysis will help identify key areas requiring attention, optimize HR interventions, and ensure a supportive work environment for all employees.

## Steps followed 


### 1. REQUIREMENTS GATHERING

###  - Identify Stakeholders
- HR Department

- Department Heads (e.g., R&D, Sales)

- Employees




### - Objectives
- Track Current Attrition Rates and Employee Status

Monitor current attrition rates across various departments.
Identify the status of employees (current or former) and understand the reasons for attrition.

Enable HR to better manage employee retention and address key issues affecting turnover.

- AnalyzecTrends in Attrition and Job Satisfaction
Examine how attrition rates and job satisfaction levels have changed over time.

Identify patterns or trends in employee turnover and satisfaction.

Differentiate between various demographic groups (e.g., by education level, gender, age) to understand specific needs and challenges.


- Detail Departmental and Demographic Profile Analysis:

Analyze attrition and satisfaction data to determine which departments have the highest turnover rates.

Investigate differences in attrition and satisfaction based on job roles, educational background, and other demographic factors.

Explore how factors such as age, gender, and education influence employee retention and satisfaction to identify key areas for intervention.

### - Scope of the Study



- Project Scope: Includes tracking current attrition rates, analyzing historical trends, and performing detailed analyses by department and demographic profiles..

- Limitations: The analysis is based on the available dataset and does not include real-time data. The study focuses on identifying trends and patterns to inform strategic HR decisions.

### 2. DATA COLLECTION

- Data Source: Used a excel as a data connector to collect HR data.
- Loading Data: Loaded the data into Power BI for further processing and analysis.

### 3. DATA TRANSFORMATION

- Ensure Correct Data Types:
Verified that all data types are in the correct format.


- Data Validation:
Ensure that every row and Column has correct data

- Standardize Outpatient Data:
Added a new column, "Case_type," to the outpatient data to match the structure of the inpatient data.

 ### 4. DATA MODELLING
There was no need for data modeling as the data consisted of a single table.

 ### 5. DATA VISUALIZATION
1. Key Performance Indicators (KPIs):

    Total number of Employees:
Found the count of overall Employees and used card on Power BI

Snap of Total Number of Employees

![1](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/50703873-0a36-4206-8224-b42b6b260254)

2.  Attrition(Number of employees who have left the company):
 
        Calculation:
          

        in the table, "Yes" represents employees who left the company, and 
        "No" represents those who stayed.

        Create a conditional column:
        If attrition equals "Yes" then 1, else 0.
        Change the data type of the new column from text to whole number.
        This new column will provide the attrition summation.
        Click OK, then Close and Apply.Snap of Total Number of Employees


Snap of Attrition Count:

![2](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/c8e1b0ab-054d-42ef-ab27-815cef9cf445)



3.  Attrition Rate:


  

            DAX EXPRESSION:

           Attrition Rate = SUM(Sheet1[Attrition Count])/SUM(Sheet1[Employee Count])


Snap of Attrition Rate

![3](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/094f8971-dd1f-4fb1-9879-1c4d3a377c79)



4.  Active Employees:


            Active Employees = SUM(Sheet1[Employee Count]) - SUM(Sheet1[Attrition Count])



Snap of Active Employees

![4](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/6bc3c653-e458-4e4c-93cc-ba483fff44fb)

5. Average Age:

Use the field "Sum of Age" to calculate the average age of employees.

Snap of Average Age

![5](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/a6669e71-722b-4814-a1da-d578e77d1ff0)





6. Visualization Creation:

-  Pie Chart:

Created a Pie Chart to show department-wise attrition rates.

Snap of Pie Chart

![6](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/b5437039-3976-4795-b5e1-65665f1ebc0a)

-  Stacked Column Chart:

Created a Stacked Column Chart to show the number of employees by age band and gender.

Sorting the column using a conditional column:

If CF_band age equals "Under 25" then 1

Else if CF_band age equals "25-34" then 2

Else if CF_band age equals "35-44" then 3

Else if CF_band age equals "45-54" then 4

Else 5

Rename to "sort_age" and use "Sort by" to sort it in ascending order.


Snap of Stacked Column Chart

![7](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/3652cc9c-6829-4dcf-a134-00870e7f8eac)

-  Matrix Map::

Use the Matrix Map to show:

Rows: Job Roles
Values: Job Satisfaction Levels and Employee Count for each satisfaction level and job role.

Snap of Matrix Map

![8](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/a9bc3736-8d6e-423a-a8f1-812fbb1cab6e)

-  Horizontal Bar Chart:

Created a Horizontal Bar Chart to show the attrition count by level of education.

Snap of horizontal bar Chart

![9](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/5df91ee2-c025-4575-99c7-a1be620f937e)



-  Donut Chart:

Created a Donut Chart to display attrition rate by gender and age groups.

Use cards to show the attrition count of each age group inside the chart.

Snap of Donut Charts

![10](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/449e345c-c39b-487b-865d-3442679f8bf2)


7. Build Aesthetics:

Canvas Background:
I changed the canvas background using MS PowerPoint to enhance the visual appeal.

I ensured that the background complemented the overall theme and was not too distracting.

8. Interactivity:

Edit Interactions:
I enabled edit interactions to ensure every visual was interactive with each other.
This ensured that selections in one visual filtered the data in the other visuals, providing a more dynamic and insightful user experience.

 
 # Report Snapshot (Power BI DESKTOP)

 
![EMPLOYEE ATTRITION](https://github.com/TheDataVirtuoso/CollinsBahati.github.io/assets/87636760/ed2d3f4d-bf73-4671-9f64-bf6f48c3538f)


# Insights and Recommendations

A One page report was created on Power BI Desktop 

Following inferences can be drawn from the report;

### [1] Attrition Rate Overview:

   The overall attrition rate in the company is 16.12%, indicating that approximately 16 out of every 100 employees leave the company.


    Recommendation: Regularly monitor the overall attrition rate to identify
    any significant changes. Implement company-wide retention strategies such 
    as enhancing career development opportunities, improving workplace culture, 
    and offering competitive benefits.
           
### [2] Departmental Attrition:


  
 The Research and Development (R&D) department, despite having the highest number of employees (961), experienced a relatively high attrition rate of 13.84%, with 133 employees leaving.


    Recommendation: Conduct a detailed analysis of the R&D department to identify specific
    factors contributing to attrition. This could include employee surveys, exit interviews, 
    and workload assessments. Implement targeted interventions such as mentorship programs, 
    workload balancing, and career advancement opportunities.
  
  ### [3] Education Level and Attrition:
  
Employees with a bachelor's degree had the highest attrition rate at 17.31%.


    Recommendation: Investigate why employees with bachelor's degrees are more prone to leaving. 
    Possible actions include providing advanced training opportunities, clear career progression 
    paths, and recognizing their contributions to increase job satisfaction and retention.

 ### [4] Gender and Attrition:
Male employees had the highest attrition count of 150


    Recommendation: Explore the reasons for higher attrition among male employees. 
    Consider implementing flexible work policies, targeted retention programs, 
    and creating an inclusive work environment that addresses the specific 
    needs and concerns of male employees.

 ### [5] Job Role and Job Satisfaction:

Lab technicians had a high job satisfaction rating of 259.

    Recommendation: Analyze the factors contributing to high job satisfaction among lab 
    technicians, such as job roles, work environment, and management practices. 
    Apply these successful practices to other roles and departments to improve 
    overall job satisfaction and retention.


### [5] Average Age of Employees:

The average age of employees in the company is 36.92.

    Recommendation: Utilize this demographic overview to tailor retention 
    strategies that cater to different age groups. Consider implementing 
    programs that address the specific needs and preferences of younger 
    and older employees, such as career development for younger employees 
    and work-life balance initiatives for older employees. 
