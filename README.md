Displaying Records from the Table: You first used the SELECT * FROM info query to display all the records in the info table, showing employee details such as eid (employee ID), ename (employee name), and esal (employee salary).

Inserting a New Record: You inserted a new employee (eid=8, ename='abhi', esal=2345.65) into the info table using the INSERT INTO info VALUES statement.

Deleting a Record: You deleted an employee with a salary of 356 using the DELETE FROM info WHERE esal=356.

Updating a Record: You tried updating the salary of an employee named chetan using the UPDATE statement, although this employee was not present in the current data. However, the query still showed success, meaning it matched 1 row, even though it’s not reflected in the data.

Counting Rows: You used both COUNT(eid) and COUNT(*) to count the total number of rows in the table, and both returned 7.

Average, Minimum, Maximum Calculations:

You calculated the average salary using AVG(esal), which resulted in 1657.9813973563057.
You also calculated the minimum (345) and maximum (3445.45) salaries using MIN(esal) and MAX(esal) respectively.
Additionally, you found the average employee ID (AVG(eid)), which resulted in 4.4286.
Identifying Employee with Minimum Salary: You found the employee (priti) with the minimum salary (345) using a subquery in the WHERE clause.

Displaying Employees and Their Departments (Joining Tables):

You used an inner join, left join, and right join to combine the info and dinfo tables based on eid to display department (dname) and employee name (ename). The results varied based on the join type:
Inner Join showed records where there were matching eids in both tables.
Left Join included all rows from dinfo and matched rows from info.
Right Join included all rows from info and matched rows from dinfo.
Creating a View: You created a view named esal that holds all employees with a salary less than or equal to 1000. The view included three employees (janhavi, ritika, priti).

Creating a Function: You created a user-defined function (add_status) to classify salaries into categories (low, medium, high) based on their values. This function was used in a SELECT query to display the status of each employee's salary:

Salaries ≤ 1000 were classified as "low."
Salaries between 1000 and 3000 were classified as "medium."
Salaries ≥ 3000 were classified as "high."
The final query applied this function and returned the salary status for each employee.
