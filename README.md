# Pewlett_Hackard_Analysis

## Overview & Purpose of the Project 
After exploring the company data, creating a database in pgAdmin4 with SQL, sorting and generating lists of employees eligible for retirement by department, we were tasked to determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program to help the manager prepare for the upcoming "silver tsunami."

## Deliverables
## 1: The Number of Retiring Employees by Title

Using the ERD you created in this module as a reference and your knowledge of SQL queries, create a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions—you’ll need to use the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, use the COUNT() function to create a table that has the number of retirement-age employees by most recent job title. Finally, because we want to include only current employees in our analysis, be sure to exclude those employees who have already left the company.

![Retirement_Titles](Resources/Retirement_Titles.png)

![Unique_Titles](Resources/Unique_Titles.png)

![Retiring_Titles](Resources/Retiring_Titles.png)

## 2: The Employees Eligible for the Mentorship Program

Using the ERD you created in this module as a reference and your knowledge of SQL queries, create a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965.

![Mentorship_Eligibility](Resources/Mentorship_Eligibility.png)

## 3: Analysis

### Results

Provide a bulleted list with four major points from the two analysis deliverables. Use images as support where needed.

-
-
-
-


### Summary

Provide high-level responses to the following questions, then provide two additional queries or tables that may provide more insight into the upcoming "silver tsunami."

How many roles will need to be filled as the "silver tsunami" begins to make an impact?

Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
