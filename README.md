
# Student Record Management System

A C-based program with login authentication and role-based access control (Admin, Staff, User, Guest).
This system manages students using a text-file–based database.

## Features
- Login system with roles
- Add, display, search, update, delete student records
- Role-based menu access

## Roles
- Admin: Add, Display, Search, Update, Delete
- Staff: Add, Display, Search, Update
- User: Display, Search
- Guest: Display, Search

## Files
- student_app.c
- credentials.txt
- students.txt

## How to Run
```
gcc student_app.c -o student_app
./student_app
```
