📘 Student Record Management System

A complete C-based student management software with user authentication, role-based access, and file-based storage.
This project demonstrates file handling, modular programming, user authentication, and data management in C.
It is perfect for college mini-projects, file handling labs, and anyone learning C language.

📑 Table of Contents

Introduction

Features

System Requirements

Project Structure

How It Works

User Roles & Permissions

Data File Formats

Compilation & Execution

Program Flowchart

Sample Screenshots

Future Enhancements

About The Project

📖 Introduction

The Student Record Management System is built to perform basic operations like:

Adding student data

Displaying all students

Searching by roll number

Updating an existing record

Deleting a student record

It uses text files for data storage instead of databases, making it easy to use anywhere.

✨ Features
🔐 Login System

This project uses a username + password system.
All credentials are stored in a file: credentials.txt.

👥 Role-Based Access

Multiple roles are supported.
Each role has defined permissions.

📁 File Handling

Data is saved permanently using:

students.txt → Student database

credentials.txt → User credentials

🧾 Student Operations

Add Student

Display All Students

Search for a Student

Update Student Information

Delete a Student (Admin only)

🖥 System Requirements

Any OS: Windows, Linux, macOS

GCC or a C compiler

Terminal/Command Prompt

📂 Project Structure
Student_Record_Management_System/
│
├── README.md               # Documentation
├── student_app.c           # Main program source code
├── credentials.txt         # Login details for users
└── students.txt            # Student database

🔍 How It Works
Program Flow

User runs the program

Login screen appears

Program checks credentials.txt

If login is correct → loads role menu

User performs allowed operations

Data stored in students.txt

Logout ends session

👥 User Roles & Permissions
Feature	Admin	Staff	User	Guest
Add	✔	✔	✘	✘
Display	✔	✔	✔	✔
Search	✔	✔	✔	✔
Update	✔	✔	✘	✘
Delete	✔	✘	✘	✘

📝 Data File Formats
🔐 credentials.txt
username password role

Example:

admin admin123 admin
staff staff123 staff
user user123 user
guest guest123 guest

🧾 students.txt
roll name marks

Example:

1 John 78.5
2 Maya 88.0
3 Alex 90.0

⚙ Compilation & Execution
Compile
gcc student_app.c -o student_app

Run
./student_app

📊 Program Flowchart
          ┌──────────────┐
          │    START      │
          └───────┬──────┘
                  │
        ┌─────────▼─────────┐
        │   LOGIN SCREEN     │
        └─────────┬─────────┘
                  │Valid?
      ┌───────────┴────────────┐
      │         NO              │
      │ "Invalid Login" Message │
      └───────────┬────────────┘
                  │YES
        ┌─────────▼─────────┐
        │ Load Role Menu     │
        └─────────┬─────────┘
                  ▼
        ┌────────────────────┐
        │ Perform Operations  │
        └─────────┬─────────┘
                  ▼
          ┌──────────────┐
          │    LOGOUT     │
          └───────┬──────┘
                  ▼
          ┌──────────────┐
          │     END       │
          └──────────────┘

🖼 Sample Screenshots (Text Output)
Login Screen
=====================================
       STUDENT RECORD SYSTEM
=====================================
USERNAME : admin
PASSWORD : admin123

✔ Login successful! Logged in as: admin

Admin Menu
============== ADMIN MENU ==============
1. Add Student
2. Display All
3. Search
4. Update
5. Delete
6. Logout

Display Output
ROLL    NAME            MARKS
--------------------------------
1       John            78.50
2       Maya            88.00
3       Alex            90.00

🚀 Future Enhancements

Possible improvements:

Hide password input (****)

Sorting table (by marks/name/roll)

Statistics (total students, average marks)

Backup system

Pagination for long data

GUI using Tkinter/Qt

CSV export

Colorful terminal UI

Tell me if you want any of these features—I can add them.

ℹ About This Project

This project is best for:

Computer Science students

C programming course work

Demonstrating file handling

Mini projects for diploma/degree

Easy to understand, modify, and submit.
