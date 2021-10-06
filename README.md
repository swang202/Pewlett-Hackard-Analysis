# Pewlett-Hackard-Analysis

###Overview of the analysis:

The purpose of the analysis is to determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. Data was store and analysed using PostgreSQL database.


###Results:
1. Retiring employees and their title
	- In order to retrieve the titles for employees that fits the retirement criteria, we merged the employees table and the title tables by "employee number" for employees that are born between _January 1st of 1952_ to _December 31st of 1955_. 
	- Employees might contains multiple titles during their years in the company.
	- To retrieve the current title of retiring employees, we sort the to_date in descending order and retrieve the first occurrence of the employee number. 
	- Total number of retiring employees by title was summarized. 

2. Mentorship eligibility
	- To identify employees who are eligible to participate in a mentorship program. We first selected employees who are employed currently using to_date, and are born between _January 1, 1965_ and _December 31, 1965_. Employee titles were listed.
	
###Summary:

- 90398 Employees who fit the retiring requirement with current title were listed, including 29414 senior engineers, 28254 senior staffs and 2 managers.
- 1549 current employees that are eligible for mentorship program.