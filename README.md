# -dbms-assignment-lab2.sql
College Database ER Diagram with relational schema and Oracle SQL Plus queries
# College Database Management System

## Overview
This repository contains the *Oracle SQL*Plus implementation* of a College Database Management System (DBMS) along with the *ER Diagram*.  
The project demonstrates the creation of relational tables, establishing relationships, primary and foreign keys, and many-to-many relationships using an associative table.

---

## *Contents*
1. *ER Diagram*  
   - Shows all entities: Department, Student, Faculty, Course, Enrollment  
   - Displays relationships and cardinality  
   - Enrollment table resolves the many-to-many relationship between Students and Courses  

2. *SQL File* (CollegeDB.sql)  
   - Contains CREATE TABLE statements for all entities  
   - Includes constraints: Primary Keys, Foreign Keys, Unique constraints  
   - Ready to run in Oracle SQL*Plus  

---

## *Database Structure*

### *Tables*
1. *Department*  
   - DepartmentID (PK), DepartmentName, OfficeLocation

2. *Faculty*  
   - FacultyID (PK), Name, Designation, Email (Unique), DepartmentID (FK)

3. *Student*  
   - StudentID (PK), Name, DateOfBirth, Gender, ContactNumber, DepartmentID (FK)

4. *Course*  
   - CourseID (PK), CourseName, Credits, DepartmentID (FK), FacultyID (FK)

5. *Enrollment*  
   - EnrollmentID (PK), StudentID (FK), CourseID (FK), Semester, Grade  
   - Resolves many-to-many relationship between Students and Courses

---

## *How to Use*

1. Open Oracle SQL*Plus.
2. Run the SQL file:
   ```sql
   lab2_solution.sql
