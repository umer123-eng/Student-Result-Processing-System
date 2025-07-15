# 🎓 Student Result Processing System – Day 1

## 🔰 Day 1: Database Planning & Design

This repository contains the foundational database schema and ER model for the **Student Result Processing System** project.

---

## 🎯 Objectives
- Design a normalized relational database system to manage:
  - Student information
  - Course registration
  - Marks and grade calculation
  - GPA & CGPA computation

---

## 📋 Tasks Completed

✅ **1. Requirement Understanding**
- Identify core entities: Students, `Courses,Results, Grades, StudentCourses,Semester
- Attributes like: `marks`, `grades`, `exam_type`, `credit_hours`

✅ **2. ER Diagram Created**
- ER model shows relationships:
  - One-to-many (Students → Results)
  - Many-to-many (Students ↔ Courses via `StudentCourses`)
  - Grade table used for calculating GPA from marks

✅ **3. Table Design & Schema**
- Created the following tables:
  - Students
  - Courses
  - Semester
  - StudentCourses (Enrollment)
  - Results
  - Grades
  - GPA

✅ **4. Relationships**
- Primary Keys and Foreign Keys defined for referential integrity

---

## 🗂️ Files in this Repo

| File Name             | Description                                 |
|----------------------|----------------------------------------------|
| schema.sql           | SQL script to create all required tables     |
| er-diagram.png       | Exported EER diagram from MySQL Workbench    |
| README.md            | This file – project overview and Day 1 plan  |

---

## 🛠 Tools Used
- MySQL Workbench
- ER Diagram Designer (Workbench canvas)

---

## 📌 Notes
- Schema is normalized to avoid redundancy
- Designed for scalability (future semester-wise GPA tracking, etc.)

---

## 👨‍💻 Created By

**Umer Mansuri**  
Intern @ Elevate Labs | July 2025


# 🎓 Student Result Processing System – Day 2

## 🔰 Day 2: Insert Data + Views

This part of the project focuses on inserting data into the database, executing JOIN-based queries, and creating reusable views to analyze student performance.

---

## 🎯 Objectives

- Insert sample data into all relational tables
- Use JOINs for reporting and analysis
- Create **Views** for simplified query access
- Add **advanced SQL operations** using aggregates and subqueries

---

## 📋 Tasks Completed

### ✅ 1. Data Insertion
All tables populated using INSERT INTO:
- Students
- Courses
- Semester
- StudentCourses
- Results
- Grades

✅ All data saved in data.sql

---

### ✅ 2. Queries with JOINs
Created complex SELECT queries for:

- Student-wise subject performance  
- Course-wise average, max, min marks  
- Exam-type filters (e.g., Final only)  
- GPA computation using `Grades` table  
- Listing students who failed  
- Course toppers using subqueries

✅ All queries saved in queries_day2.sql

---

### ✅ 3. Views Created

| View Name                 | Description                                      |
|-------------------------  |--------------------------------------------------|
| view_student_results      | Full result details per student per subject      |
| view_course_performance   | Avg marks and attempts per course                |
| view_distinction_students | Students who scored 75+ in any subject          |

✅ View scripts are also saved in `queries_day2.sql`

---

## 💡 Advanced Queries Added

- 📌 **Topper Selection** – Highest scorer in each subject  
- 📌 **GPA Calculation** – Average grade point using JOIN + GROUP BY  
- 📌 **Failed Students** – Students scoring less than 40 marks  
- 📌 **Final Exam Only** – Filtering exam results by type  
- 📌 **View for Distinction Students** – Marks ≥ 75

---

## 🗂️ Files in this Repo

| File Name           | Description                                        |
|---------------------|----------------------------------------------------|
| data.sql            | Insert data for all tables                         |
| queries_day2.sql    | SELECT + JOIN queries + all views                  |
| README.md           | This project overview for Day 2                    |


---

## 🛠 Tools Used

- MySQL Workbench
---

## 👨‍💻 Created By

**Umer Mansuri**  
Intern @ Elevate Labs | July 2025





