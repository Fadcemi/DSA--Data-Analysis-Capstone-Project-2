# DSA--Data-Analysis-Capstone-Project-2
PowerBI Case study solutions

# Problem Satement
  The Palmoria Group, a manufacturing company based in the Nigeria is embroiled in issues bordering on gender inequality in its 3 regions. Unfortunately, the media recently published in the news with the headline “Palmoria, the Manufacturing Patriarchy” This doesn’t look good for the owners of the business based on their ambition to scale the business to other regions and even overseas. Cases like this can only spiral downwards revealing other issues like gender pay gap amongst other possible issues.

  As an HR Analytics expert, I was assigned the task to analyze the company’s HR data to identify key areas within the business that could spring up issues and come up with recommendations for management’s attention and give a breakdown of the Salary details.

  “Now, the future of gender equality in Palmoria lies in your hands” the exact words of Mr. Shofoluwe before he handed the data to me.

# Objective
● Focus is on gender related issues within the organization and its regions
1. Gender distribution in the organization
2. Insights on ratings based on gender
3. Company’s salary structure. To identify if there is a gender pay gap. If there is, the department and regions that should be the focus of management.
4. If Palmoria meets the requirement of manufacturing companies paying employees a minimum of #90,000
5. Pay distribution of employees grouped by a band of #30,000.
5. Allocation of the annual bonus pay to employees based on the performance rating.
- Amount to be paid as bonus to individual employees
- Total amount to be paid to individual employees (salary inclusive of bonus)
- Total amount to be paid out per region and company-wide


# Data Sourcing
Dataset and Project Brief can be gotten [here]()

# Data Transformation
● I loaded the employee dataset into Power Query which had 6 columns 1016 rows

● I assigned a generic gender status (Undisclosed) to employees that refused to disclose their gender.

● I removed employees without salary (because it indicates they are no longer with the company), departments that indicated as “NULL”. I also removed duplicates from the dataset thus giving us 6 columns 943 rows

● I had to get the bonus salary for each employee,so I loaded the bonus details dataset which had 6 columns and 12 rows. I unpivoted the rating columns givng me a total of 3 columns and 60 rows after which I then merged both the bonus details and employee details together using department and rating column. Leaving us with 7 columns 943 rows. (Since I merged already, I disabled the bonus dataset from loading into powerbi)

● I then loaded into powerbi desktop 

● I created some new measures to help in my analysis

● I also created a new column 'Salary Range' to group the salaries in a band of #30k
