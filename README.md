# Pewlett Hackard Analysis
## Overview of the analysis:
The Objective of this project is to determine the number of retiring employees per title and identify employees who are eligible to participate in a mentorship program. For this, we used the company's employees data set which can be found in the Data folder.

### Programs used
- SQL

We had to wrangle the original dataset using SQL to filter out the information we did not need and then create new tables that allowed us to perform different analysis. The script used for this can be found on the Queries folder. 

## Results: 
The results we found are provided below:
1. There are 90.398 employees who will retire, which of 1940 are eligible for the mentorship program.
2. Pewlett Hackard has 300,024 emplyees, so the employees who will be retiring represents the 30.13%.
3. The position with the most retireing employees is Senior Engineer.
4. The corresponding percentages of retiring employees for each title is: Senior Engineer 32%, Senior Staff 31%, Engineer 16%, Staff 14%, Technique Leader 5%, Assistant Engineer 2%, Manager less than 1%. 

![](/Resources/retiring_titles.png) 

In the following pie graph you can see a breakdown of the different departments and what percentage of their staff will be retiring. 
![](/Resources/retiring_titles_pie.png)

## Summary: 
How many roles will need to be filled as the "silver tsunami" begins to make an impact? 
The company will need to fill 90.398 positions or 30.13% of their total employee population. We can apply a count query to the unique_titles.csv table to get the total amount of employees that will retire. 


![](/Resources/unique_titles_count.png)

The total amount of employees that are qualified for the mentorship program is 1940, which represents the 0.64% of the total employees. With this numbers, each retired employee would have to mentor 155 employees. We can determine that there are not enough qualified employees to mentor the next generation of Pewlett Hackard employees. To get the total amount of employees that are eligible for the mentorship program we can apply a filter to the retiring_titles.csv and then a count selec query and we get the following table as a result:  
![](/Resources/mentorship_eligibility_count.png)
