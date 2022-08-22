# Employee Database

## Background

This is a research project on employees of the corporation from the 1980s and 1990s. All that remains of the database of employees from that period are six CSV files.

We designed the tables to hold data in the CSVs, imported the CSVs into a SQL database, and answered questions about the data. In other words, we performed **data modeling**, **data engineering**, and **data analysis**.

#### Data Modeling

After inspecting the given CSVs we sketched the ERD of the tables using a free tool [http://www.quickdatabasediagrams.com](http://www.quickdatabasediagrams.com).

#### Data Engineering

* Using the provided information to create a table schema for each of the six CSV files. We will specify data types, primary keys, foreign keys, and other constraints.

  * Primary keys are assigned to the column that is unique. Otherwise, a [composite key](https://en.wikipedia.org/wiki/Compound_key) is created, which takes two primary keys to uniquely identify a row.

* Imported each CSV file into the corresponding SQL table. 

#### Data Analysis

Once we have a complete database, following steps are prefomed for analysis:

1. Listed the following details of each employee: employee number, last name, first name, sex, and salary.

2. Listed first name, last name, and hire date for employees who were hired in 1986.

3. Listed the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name.

4. Listed the department of each employee with the following information: employee number, last name, first name, and department name.

5. Listed first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B."

6. Listed all employees in the Sales department, including their employee number, last name, first name, and department name.

7. Listed all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.

8. Listed the frequency count of employee last names (i.e., how many employees share each last name) in descending order.

## Visual Analysis in Pandas

To create a visualization of the data in Jupyter NB, following steps are prefomed:

1. Imported the SQL database into Pandas using [SQLAlchemy](https://docs.sqlalchemy.org/en/latest/core/engines.html#postgresql). 

2. Created a histogram to visualize the most common salary ranges for employees.

3. Created a bar chart of average salary by title.

## Files

* [Image File](sql_challenge/employee_db_ERD.png) showing ERD.

* [Create Table](sql_challenge/employee_table_sch.sql) for table schemata.

* [SQL Query](sql_challenge/queries.sql) for data analysis.

* [Jupyter notebook](sql_challenge/sqlalchemy.ipynb) for visual analysis.




