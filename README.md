# sql-challenge
# Background
It’s been two weeks since you were hired as a new data engineer at Pewlett Hackard (a fictional company). Your first major task is to do a research project about people whom the company employed during the 1980s and 1990s. All that remains of the employee database from that period are six CSV files.

For this project, you’ll design the tables to hold the data from the CSV files, import the CSV files into a SQL database, and then answer questions about the data. That is, you’ll perform data modelling, data engineering, and data analysis, respectively.

## Before Begin
Create a new repository for this project called sql-challenge. Do not add this assignment to an existing repository.

Clone the new repository to your computer.

Inside your local Git repository, create a directory for this Challenge. Use a folder name that corresponds to the Challenge, such as EmployeeSQL.

Note that you’ll add your files to this folder and push the changes to GitHub.

## Files
Download the following files to help you get started:

Module 9 Challenge filesLinks to an external site.

## Instructions
This Challenge is divided into three parts: data modelling, data engineering, and data analysis.

## Data Modelling
Inspect the CSV files, and then sketch an ERD of the tables. To create the sketch, feel free to use a tool like QuickDBD Links to an external site..

## Data Engineering
Use the provided information to create a table schema for each of the six CSV files. Be sure to do the following:

Remember to specify the data types, primary keys, foreign keys, and other constraints.

For the primary keys, verify that the column is unique. Otherwise, create a composite key Links to an external site., which takes two primary keys to uniquely identify a row.

Be sure to create the tables in the correct order to handle the foreign keys.

Import each CSV file into its corresponding SQL table.

HINT
## Data Analysis
List the employee number, last name, first name, sex, and salary of each employee.

List the first name, last name, and hire date for the employees who were hired in 1986.

List the manager of each department along with their department number, department name, employee number, last name, and first name.

List the department number for each employee along with that employee’s employee number, last name, first name, and department name.

List the first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.

List each employee in the Sales department, including their employee number, last name, and first name.

List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.

List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).

Bonus
As you examine the data, you begin to suspect that the dataset is
fake. Maybe, your boss gave you spurious data to test the data
engineering skills of a new employee? To confirm your hunch, you
decide to create a visualisation of the data to present to your boss.
To do so, complete the following steps:
1. Import the SQL database into Pandas. (Although you could
read the CSV files directly in Pandas, you’re trying to prove
your technical resourcefulness.) Note that this step might
require some research. Feel free to use the following code to
get started (where &lt;your_db_name&gt; is your database name):

2. from sqlalchemy import create_engine

3. engine = create_engine(&#39;postgresql://localhost:5432/&lt;your_db_name&gt;&#39;)

4. connection = engine.connect()

NOTE
For more information about the create_engine function, see
the SQLAlchemy documentationLinks to an external site..
If you’re using a password, don’t upload it to your GitHub
repository. For more information, review the Oops! I
Committed My Password To GitHub!Links to an external
site. video and Ignoring filesLinks to an external site. in
GitHub Docs.
5. Create a histogram to visualise the employee salary ranges
that were the most common.
6. Create a bar chart of average salary by title.

## Requirements
Data Modelling (10 points)
Entity Relationship Diagram is included or table schemas provided for all tables (10 points)
Data Engineeing (70 points)
All required columns are defined for each table (10 points)
Columns are set to the correct data type (10 points)
Primary Keys set for each table (10 points)
Correctly references related tables (10 points)
Tables are correctly related using Foreign Keys (10 points)
Correctly uses NOT NULL condition on necessary columns (10 points)
Accurately defines value length for columns (10 points)
Data Analysis (20 points)
List the employee number, last name, first name, sex, and salary of each employee (2 points)
List the first name, last name, and hire date for the employees who were hired in 1986 (2 points)
List the manager of each department along with their department number, department name, employee number, last name, and first name (2 points)
List the department number for each employee along with that employee’s employee number, last name, first name, and department name (2 points)
List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B (2 points)
List each employee in the Sales department, including their employee number, last name, and first name (2 points)
List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name (4 points)
List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name) (4 points)

Before submitting your Challenge assignment, make sure that you’ve done the following:

Create an image file of your ERD.

Create a .sql file of your table schemata.

Create a .sql file of your queries.

(Optional) Create a Jupyter notebook of the bonus analysis.

Ensure that your repository has regular commits and a thorough README.md file
