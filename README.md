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

