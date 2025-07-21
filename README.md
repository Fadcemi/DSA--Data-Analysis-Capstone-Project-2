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
4. If Palmoria meets the requirement of manufacturing companies paying employees a minimum of $90,000
5. Pay distribution of employees grouped by a band of $10,000.
5. Allocation of the annual bonus pay to employees based on the performance rating.
- Amount to be paid as bonus to individual employees
- Total amount to be paid to individual employees (salary inclusive of bonus)
- Total amount to be paid out per region and company-wide


# Data Sourcing
Dataset and Project Brief can be gotten [Here](https://github.com/Fadcemi/DSA--Data-Analysis-Capstone-Project-2/blob/main/MY%20PROJECT.pbix)

# Data Transformation
● I loaded the employee dataset into Power Query which had 6 columns 1016 rows

● I assigned a generic gender status (Undisclosed) to employees that refused to disclose their gender.

●  Employees without salary (because it indicates they are no longer with the company) and departments that indicated as “NULL” were removed.  Also removed are duplicates from the dataset thus giving us 6 columns 923 rows

● In order to get the bonus salary for each employee, I loaded the bonus mapping dataset which had 6 columns and 12 rows, unpivoted the rating columns giving me a total of 3 columns and 60 rows. The bonus details and employee details were merged using department and rating columns. Finally those not rated were assigned zero(0),
leaving us a cleaned table with 7 columns 923 rows. 

● I then loaded into powerbi desktop 

● I created some new measures to help in ascertaining the average, minimum salary etc

● I also created a new column 'Salary Range' to group the salaries in a band of #10k

# Data Visualisation
![All images](https://github.com/user-attachments/assets/ff3d0652-567d-46c1-911c-f8c4026ae72a)




# Analysis

⚠ N.B: The undisclosed gender category may affect the accuracy of this analysis. However, they make up only about 4.23% of the total employees.

### Gender Distribution
  ● General Overview

There is a total of 923 employees, 452 Males, 432 Females and 39 undisclosed.


![gender distribution by region ](https://github.com/user-attachments/assets/902bad9f-ef77-4b35-8b76-efff93683c56)

Gender distribution is fair in the company with Males being 2% more than females and about 4.23% of employees did not disclose their gender.

  ● Regions
  
Abuja has a balanced proportion of Males and Females with 154 each.

Kaduna is the region with the widest gender gap with 15 more Males than Females.

Lagos also has 5 more Males than Females.


  ● Department
  
![gender distribution](https://github.com/user-attachments/assets/a13749d0-94e6-454f-bc23-b4e818e61e22)

Considering Male and Female Gender, Legal, Accounting and Support are departments with the most gender gaps dominated by males.

In Marketing, Engineering, Product Management and Training, the gender is fairly distributed.

Futher analysis shows that Services and Research and development are departments where the Females are more than Males.


### Rating
Tho Rating was fairly distibuted among the genders.

Males dominated the very poor,poor and average rating while females lead in the not rated, good and very good category.

![rating](https://github.com/user-attachments/assets/d29e8587-1557-43ca-b77c-aebb427be4cc)

### Salary
  ● General Overview
  
Total of the New Salary to be Paid out by the company is $70.712M including bonus, bonus salary is about $2.14M while salary without bonus is $67.98M

The average salary is $75.97k

![salary structure](https://github.com/user-attachments/assets/5b6c8aae-330a-448d-899c-634d0d56319c)

Average salary among the genders is fairly distributed

  ● Regions
  
Kaduna Total Salary is $26.79M, Abuja is $24.17M and Lagos Total Salary is $19.15M

  ● Department
  
In most departments, the Males earn more except 3 departments where females earn more that is Training, Marketing and Engineering

  ● Salary Range
  
Grouping the salaries by a band of #10k. Most employees earn within the range 70k to 80k, and least earn within 20k to 30k.


![range](https://github.com/user-attachments/assets/37b3fa9b-8830-497b-b845-e70cb403e41e)

  ● Minimum Salary requirment
  
Considering the recent regulation which requires manufacturing companies to pay employees a minimum of $90,000.

Palmoria group falls short of this, with about 69.12% of the workers earning less than the minimum requirment

![range by dept](https://github.com/user-attachments/assets/fe4c5a42-d748-4d43-931f-a957c827488d)

  ● Computation for the bonus and New Salary
  
  ![table](https://github.com/user-attachments/assets/eb330e98-f8b9-4c3c-84dc-0a008c9000a6)


# Findings
•	Gender is fairly distributed throughout the organization.

•	Kaduna region has the widest gender gap, followed by Lagos while distribution is equal in Abuja.

•	Legal, Accounting and Support departments has a wide gender gap in favour of male.

• Marketing, Engineering and Training department gender is fairly distributed.

•	Average salary for the employees is fairly distributed among the genders.

•	In most departments the pay gap is more than 5% between both male and female gender.

•	More males earn more than the minimum requirment($90,000) compared to females.

•	Employees ratings are fairly distributed across the genders.

•	Majority of the employees earn salaries below the minimum requirement 


# Recommendation
•	Gender distribution should be improved in Kaduna region.

•	Gender distribution should also be improved in Legal, Accounting and Support.

•	The salary structure should be reviewed to ensure the minimum salary requirement is met.

•	The salary gap between males and females should be reviewed for fairness.

•	Survey should be carried out to find out why the females have better ratings than the males, and plans should be in place to train the employees.
