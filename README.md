# Final-Project_SQL
The final project of MTA Database Fundamentals course.
## The Objective
*	Use “Grade Record” dataset (either use the entire dataset or the first 50 record).
*	Create a master table that will hold your entire dataset.
*	Normalize the dataset into third normal form.
*	Identify primary and foreign keys for your tables.
*	Use JOIN to create a consolidated table.
*	Present your code to class.
## Implementation
### Conceptual Design (ERD). Define PKs and FKs to ensure referential integrity. 
the Master table was broken down into 3 tables: Students, Exams, Final Grades to comply with 2NF and 3NF
![](ERD.png)

### Relational Model. How db tables looked with all PKs and FKs assigned.
![](relational.png)

### Check for duplicate records. 
* This step was challenging as there are several methods to check for and delete duplicates and it required a thorough research to find the way that suited the best in my situation. I ended up using GROUP BY and HAVING COUNT(*) > 1 to check for duplicates and than if ound, delete them using MAX function. No duplicates found, 1NF complied.
* Several views were created using JOIN, for example, to show students who failed, who has rates 1-5, etc.
