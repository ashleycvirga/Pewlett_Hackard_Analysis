# Pewlett_Hackard_Analysis

Employee database analysis on retiring employees using SQL and pgAdmin

## Overview & Purpose of the Project 
After exploring the Pewlett Hackard company data, creating a database in pgAdmin4 with SQL, sorting and generating lists of employees eligible for retirement by department, I was tasked to determine the number of retiring employees per title, and to identify employees who are eligible to participate in a mentorship program.  This is all to help the manager prepare for the upcoming "Silver Tsunami"--the wave of Baby Boomers retiring out of the workforce. Our goal is to identify employees qualified to step into a mentorship role and train employees to fill the soon to be open roles and thus mitigate the effects to the business of having a large number of unfilled positions.

## Deliverables
## 1: The Number of Retiring Employees by Title

Using the ERD I created in the module as a reference and knowledge of SQL queries, I created a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. 

![Retirement_Titles](Resources/Retirement_Titles.png)

Some employees had multiple titles in the database so I used the DISTINCT ON statement to create a table that contains the most recent title of each employee. Thus, removing the duplicates. 

![Unique_Titles](Resources/Unique_Titles.png)

Then I used the COUNT() function to create a table that has the number of retirement-age employees by most recent job title. Finally, because we wanted to include only current employees in our analysis, I was sure to exclude those employees who have already left the company.

![Retiring_Titles](Resources/Retiring_Titles.png)

## 2: The Employees Eligible for the Mentorship Program

Looking back at the ERD I created in the module and the the tables created for the first deliverable, I created the following mentorship-eligibility table that holds all current employees who were born between January 1, 1965 and December 31, 1965. 

![Mentorship_Eligibility](Resources/Mentorship_Eligibility.png)

## 3: Analysis

### Results Summary

- According to the Retiring Titles table, employees retiring will leave open positions for 29,414 Senior Engineers, 28,254 Senior Staff, 14,222 Engineers, 12,243 Staff, 4,502 Technique Leaders, 1,761 Assistant Engineers, and 2 Managers.

- The Mentorship Eligibility table shows that there are 1,549 current employees eligible for the mentorship program.

- Out of those employees eligible  for mentorship, there are 402 Engineers, 392 Senior Staff, 332 Staff, 290 Senior Engineers, 77 Technique Leaders, and 56 Assistant Engineers.

- There are not nearly enough qualified, retirement-ready employees in all of the departments to mentor the next generation of Pewlett Hackard employees based on this data. The mentorship program is an excellent start to help Pewlett Hackard mitigate the impacts of this "silver tsunami." However much more will need to be done.

#### Recomendations

- I think it's worth noting that the criteria for selecting eligible mentors in this analysis was to be a current employee and have a birth dates between January 1, 1965 and December 31, 1965.  As of present day 2022,  This would equate the age of 57 and being a current employees--of no specified length of time--makes them qualified to be a mentor.  I would strongly advocate re-evaluating this criteria for mentorship eligibility. Frankly, I would do away with focusing on age as a criterion alltogether and focus more on years of experience in their role and years working with the company.

- I would reccomend the following tables to be used to expand mentorship eligibility criteria and fill in the necessary gap to make the mentorship program most successful:

    * Years Employed at Pewlett Hackard -- This table will include current employee names, their title, number of years employed at PH (to date - from date/365 to         convert to years format expanded to two decimal places). I'm not sure how I would do this yet, but I would find a way to sum the duration of employment for             employees who have held multiple titles.
    
    *  Years Worked Under Current Title -- This table will include current employee names, their title, number of years holding their current title. Essentially we         would start this table the same as the last but instead of sumating employment durations, we would filter for unique titles. Thus giving us all current emplyees,       their current title and the duration they've held their current title.
   
    *  Expanded Birthdate Eligibility -- This table will be built the same as the table in the second deliverable but instead I would expand the selection to those         born January 1, 1977 through December 31, 1965(age 45-57).  While age alone I feel is a poor indicator of mentorship capabilities, it is worth noting that the two     tables above do not account for the experience of individuals who may not have work for PH for very long or held their current title at PH for long.  These             individuals may have valuable experience gained elsewhere to bring to a mentorship role.

- I would argue that employees who have been with the company for a significant number of years and or who have held their current title for a significant amount of time are excellent candidates to become mentors for the mentorship program regardless of their age.  While also including employees who are wiser for their years yet may not have spent as much time working at PH also might bring their outside experience into consideration for a mentorship role. Expanding this criteria for mentorship eligibility will greatly improve the mentorship program's success in keeping the company's business flowing through the "silver tsunami."



