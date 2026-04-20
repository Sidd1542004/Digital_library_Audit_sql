Digital Library Audit System (MySQL Mini Project)
Project Overview

The Digital Library Audit System is a MySQL-based mini project designed to manage and analyze library operations in a community college.

It helps track:

Book borrowings
Overdue books
Penalty calculations
Category-wise book popularity
Inactive students

This project demonstrates practical SQL usage for data management, reporting, and auditing.

Tech Stack
Database: MySQL
Tool Used: MySQL Workbench
Language: SQL

Database Schema
Tables Used
1. Books
Stores book details
Fields: BookID, Title, Author, Category, AvailableCopies

2. Students
Stores student information
Fields: StudentID, Name, Email, Department, JoinDate, Status

3. IssuedBooks
Tracks book transactions
Fields: IssueID, BookID, StudentID, IssueDate, ReturnDate

Relationships
One Student → Many IssuedBooks
One Book → Many IssuedBooks

Key Features

Overdue Book Detection
Identifies books not returned within 14 days

Penalty Calculation
₹5 per day after due date

Category Popularity
Shows most borrowed book categories

Inactive Students Detection
Students with no activity in last 3 years

Status Update
Automatically marks inactive students


Views Implemented
vw_OverdueBooks → Overdue records
vw_PenaltyReport → Penalty calculations
vw_CategoryPopularity → Popular categories
vw_InactiveStudents → Inactive users
