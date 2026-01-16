# Online Course Management System (AWS RDS + MySQL)

## 📌 Project Overview
This project demonstrates a real-world MySQL database hosted on AWS RDS to manage
students, courses, and enrollments for an e-learning platform.

## 🛠 Tech Stack
- MySQL 8.x
- AWS RDS (MySQL)
- AWS EC2 (Client)
- SQL

## 🗂 Database Schema
- students
- courses
- enrollments

## 🔑 Key Features
- Relational database design with foreign keys
- CRUD operations using SQL
- JOIN queries for reporting
- Indexing for query optimization
- Views for simplified access
- Hosted on AWS RDS

## ☁ AWS Architecture
EC2 → RDS MySQL → Database

## 📊 Sample Queries
```sql
SELECT s.name, c.course_name
FROM enrollments e
JOIN students s ON e.student_id = s.student_id
JOIN courses c ON e.course_id = c.course_id;
