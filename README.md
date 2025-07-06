# WORKING-WITH-USER-DEFINED-FUNCTIONS-IN-SQL
SQL Intern Task 8 (6 Jul 25)

# OBJECTIVE: Stored Procedures and Functions-
The aim of this task is to understand and implement **stored procedures** and **user-defined functions** in MySQL to modularize SQL logic, making queries more reusable and manageable.

# WHAT WE ACTUALLY DID:
- Use **CREATE PROCEDURE** and **CREATE FUNCTION**
- Use **parameters** and **conditional logic**
- Create at least **one stored procedure** and **one user-defined function**

# (LET'S GET GOING..)
We worked on a sample database called `college_db` containing a `students` table.
'''CREATE TABLE students (
    student_id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    department VARCHAR(100),
    marks INT
);'''

And we provided the sample database and then:
1. Stored Procedure: GetStudentsByDepartment- It returns all students from a given department.
"CALL GetStudentsByDepartment('CSE');"

2. Function: CheckResult- It returns 'Pass' if marks >= 60, else 'Fail'.
"SELECT name, marks, CheckResult(marks) AS result_status FROM students;"
