📘 Attendance Management System
🌟 1️⃣ Description

The Attendance Management System is a modern web-based application designed to simplify and automate student attendance tracking in schools and colleges.

Instead of maintaining manual registers, this system allows teachers to digitally record and manage attendance with accuracy and efficiency.

🎯 The system enables teachers to:

✅ Mark daily attendance

📅 View attendance records by date

📊 Generate weekly defaulter lists (below 75%)

📥 Export attendance and defaulter reports to Excel

🏫 Maintain class-wise and division-wise records

✨ This system reduces paperwork, minimizes errors, and automates attendance calculations.

🛠 2️⃣ Technologies Used
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

mysql-connector-python – Database connectivity

pandas – Excel report generation

BytesIO – In-memory file handling

🗂 3️⃣ Project Structure
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
👨‍🏫 4️⃣ Panel Information
🔐 Teacher Panel

Teachers can:

🔑 Login securely

🏫 Select class & division

📝 Mark daily attendance

📊 View attendance by date

⚠ Generate weekly defaulters (<75%)

📥 Export reports to Excel

🔒 Login System

Session-based authentication

teacher_id stored in session

Can be upgraded to full authentication system with password hashing

🚀 5️⃣ Features
✅ 1. Mark Attendance

Select standard & division

Mark students as Present/Absent

Prevents duplicate attendance for the same date

✅ 2. View Attendance Records

Filter attendance using:

📅 Date

🏫 Standard

🅰 Division

Displays:

Total Students

Present Count

Absent Count

✅ 3. Export Attendance

Export daily attendance to Excel

Automatically generated file

Example file name:

Attendance_10A_2026-02-23.xlsx
✅ 4. Weekly Defaulter List

Automatically calculates last 7 days

Identifies students below 75% attendance

Displays:

Roll Number

Name

Attendance Percentage

✅ 5. Export Weekly Defaulters

Generates Excel report

Sorted by lowest percentage

Example file name:

Weekly_Defaulters_10A.xlsx
▶️ 6️⃣ How to Run the Project
🧩 Step 1: Clone the Repository
https://github.com/Sies109/Attendance-Management-System.git
🧩 Step 2: Install Dependencies
pip install flask
pip install mysql-connector-python
pip install pandas
🧩 Step 3: Setup MySQL Database

Open MySQL

Create database

Run attendance_db.sql file

🧩 Step 4: Run the Application
python app.py
🌍 Step 5: Open in Browser
http://127.0.0.1:5000/
