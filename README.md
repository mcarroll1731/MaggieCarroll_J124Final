# MaggieCarroll_J124Final
Analyzing data about salaries based on degrees, college types, and college regions. 

## Question 1: Which are the top 5 paying majors? What are the 5 lowest paying majors? (Using average of starting and mid-career salary)
|  Highest Paying  |  Average Salary  |  Lowest Paying  |  Average Salary  |
| --- | --- | --- | --- |
| Chemical Engineering | $85,100.00 | Religion | $43,050.00 |
| Computer Engineering | $83,200.00 | Education | $43,450.00 |
| Physician Assistant | $83,000.00 | Spanish | $43,550.00 |
| Electrical Engineer | $81,950.00 | Interior Design | $44,650.00 |
| Aerospace Engineer | $79,350.00 | Music | $45,450.00 |

### How I solved this:
1. In the "Degrees that pay back" sheet, make a new column called "AVERAGE_SALARY"
2. Find the average of "Starting Median Salary" and "Mid-Career Median Salary" - AVERAGE(B2, C2) and apply to column
3. Sort from highest to lowest to find the top-paying majors
4. Sort from lowest to highest to find the lowest-paying majors
!['Q1', 'Question1'](Screenshot_Q1.jpg)


## Question 2: Which career has the greatest disparity between the highest paid and lowest paid people? 
#### This question has two different ways to answer it: either the percentage difference or actual monetary difference. For example, one career might have a greater monetary disparity between the highest and lowest paid employees, but if it pays more than another career, it could have a more narrow percent difference than another career with a lesser monetary disparity in salaries. I will solve this problem considering both these disparities.

## Based on monetary difference in salary: Economics with a disaprity of $159,400.00
### How I solved this:
1. In "Degrees that pay back" column, make a new column called "Difference_HIGHLOW"
2. Make an equation that subtracts the "Mid-Career 10th Percentile Salary" column from the "Mid-Career 90th Percentile Salary" column
3. Sort this new column from highest to lowest to find the greatest disparity

## Based on percentage difference in salary: The lowest-paid Physician Assistants make 46.45% what the highest-paid Physician Assistants make, though the difference in salary is only $57,600.00
### How I solved this: 
1. In "Degrees that pay back" column, make a new column called "PERCDIF_HIGHLOW"
2. Make an equation that finds what percentage of the highest salaries that the lowest-paid graduates make. That is "Mid-Career 10th Percentile Salary" divided by "Mid-Career 90th Percentile Salary" and apply to the column.
3. Sort this new column from lowest to highest to find the greatest disparity within individual majors. 
