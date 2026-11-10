# 🏫 Student Information System

A web-based Student Information System that lets an administrator manage students, departments, instructors, courses, and course enrollments from a single dashboard.

## ✨ Features

- Admin login with session-based access
- Dashboard showing totals for students, departments, instructors, courses, and enrollments
- Full add, edit, and delete (CRUD) management for students, instructors, and courses
- Add and edit management for departments
- Enrollment management: search students by name, enroll them in courses, and record grades and enrollment dates
- Server-side input validation
- Reusable Gridview PHP class that generates the data tables

## 🛠️ Technologies

| Layer    | Technology |
|----------|------------|
| Frontend | HTML, CSS  |
| Backend  | PHP        |
| Database | MySQL      |
| Server   | XAMPP      |

## 📁 Project Structure

├── assets/          # Images and icons
├── auth/            # Login pages and authentication logic
├── collage/         # Main modules (students, departments, instructors, courses, enrollment)
│   └── controll/    # Validation and controller files for each module
├── config/          # Database connection (connection.php)
├── layout/          # Shared header and logout
├── gridview.php     # Reusable table generator class
├── index.php        # Entry point
└── student_info.sql # Database schema and sample data

## 🚀 How to Run

Install [XAMPP](https://www.apachefriends.org/) and start **Apache** and **MySQL** from the XAMPP Control Panel.
2. Copy the project folder into C:\xampp\htdocs\.
3. Open phpMyAdmin at http://localhost/phpmyadmin.
4. Create a new database named student_info.
5. Select the database, click Import, and choose student_info.sql.
6. Open the project in your browser (adjust the folder name if you renamed it):
   http://localhost/student-information-system-php/

The database connection settings are in config/connection.php (default XAMPP values: user root, empty password).

## 🔑 Demo Login

- Username: admin
- Password: admin

> These are demo credentials for local testing only.

## 🗄️ Database

The student_info database contains six tables: users, student, department, instructor, course, and enrollment.

## 📝 Notes

This is an academic project created for learning purposes. Passwords are stored in plain text, and some queries are not yet parameterized, so it should not be used in production without further security hardening.






