📘 Attendance Management System
1️⃣ Description

The Attendance Management System is a web-based application developed for schools to manage and track student attendance efficiently.

This system allows:

Teachers to mark daily attendance

View attendance records by date

Generate weekly defaulter lists (below 75%)

Export attendance and defaulter reports to Excel

Maintain class-wise and division-wise records

It reduces manual register work and automates attendance calculation.

2️⃣ Technologies Used
🔹 Frontend

HTML5

CSS3

Jinja2 (Flask Template Engine)

🔹 Backend

Python

Flask Framework

🔹 Database

MySQL

🔹 Additional Libraries

mysql-connector-python (Database connection)

pandas (Excel export)

BytesIO (Memory file handling)

3️⃣ Project Structure
attendance-system/
│
├── app.py
├── attendance_db.sql
│
├── templates/
│   ├── home.html
│   ├── login.html
│   ├── dashboard.html
│   ├── select_class.html
│   ├── mark_attendance.html
│   ├── view_attendance.html
│   ├── weekly_defaulters.html
│   └── student_list.html
│
├── static/
│   └── (CSS / Images if any)
│
└── README.md
4️⃣ Panel Information
👨‍🏫 Teacher Panel

Teachers can:

Login securely

Select class & division

Mark daily attendance

View attendance by date

Generate weekly defaulters (<75%)

Export reports to Excel

🔐 Login System

Currently:

Session-based login

teacher_id stored in session

(Can be upgraded to real teacher authentication system)

5️⃣ Features
✅ 1. Mark Attendance

Select standard & division

Mark Present/Absent

Prevents duplicate marking for same date

✅ 2. View Attendance Records

Filter by:

Date

Standard

Division

Shows:

Total students

Present count

Absent count

✅ 3. Export Attendance

Export daily attendance

Excel file generated dynamically

File name format:

Attendance_10A_2026-02-23.xlsx
✅ 4. Weekly Defaulter List

Automatically calculates last 7 days

Students below 75% attendance

Displays:

Roll number

Name

Attendance Percentage

✅ 5. Export Weekly Defaulters

Generates Excel file

Sorted by lowest percentage

File name format:

Weekly_Defaulters_10A.xlsx
