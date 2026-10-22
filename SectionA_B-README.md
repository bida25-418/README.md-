Gradebook Management System
Project Overview

The Gradebook Management System is a Python application developed for the ICT201 Introduction to Python Programming assignment. The system manages student grades and generates reports for academic performance tracking.

This implementation covers:

Section A: Scalar Objects and Loops
Section B: Lists and Tuples

The program allows users to enter student information, validate grades, calculate averages, and generate class reports for both single-subject and multiple-subject scenarios.

Features List
Section A - Scalar Objects and Loops

◾Enter the number of students

◾ Capture student names

◾ Capture grades for a single subject (PYTHON)

◾ Validate grades between 0 and 100

◾ Prevent non-numeric grade input

◾ Calculate total class grades

◾ Calculate class average

◾ Display individual student records

◾ Display class average alongside each student's grade

Section B - Lists and Tuples

◾ Support for multiple subjects:

PYTHON
DDD
IDA

◾ Store grades using lists

◾ Store student records using tuples

◾ Calculate individual student averages

◾ Display a class summary table

◾ Find highest grade in each subject

◾ Find lowest grade in each subject

◾ Display all student grades and averages

Program Architecture

Section A Data Structure

students
│
├── (name, subject, grade)
├── (name, subject, grade)
└── ...

[
    ("Theo", "PYTHON", 85.0),
    ("Mpho", "PYTHON", 91.0)
]

Section B Data Structure

students
│
├── (student_name, [python_grade, ddd_grade, ida_grade])
├── (student_name, [python_grade, ddd_grade, ida_grade])
└── ...
[
    ("Theo", [80, 75, 90]),
    ("Mpho", [95, 88, 91])
]

Input

Enter number of students: 2

Student 1
Enter student name: John
Enter grade (0-100): 80

Student 2
Enter student name: Mary
Enter grade (0-100): 90

Output

CLASS REPORT
----------------------------------------
Total Grades : 170.00
Average Grade: 85.00

Student: John Subject: PYTHON Grade: 80.00 Class Average: 85.00
Student: Mary Subject: PYTHON Grade: 90.00 Class Average: 85.00

Multiple Subject

Input

Student 1
Enter student name: John

Enter PYTHON grade (0-100): 80
Enter DDD grade (0-100): 75
Enter IDA grade (0-100): 90

Output

CLASS SUMMARY
----------------------------------------------------------------------
Name        PYTHON  DDD     IDA     Average
----------------------------------------------------------------------
John        80      75      90      81.67

SUBJECT STATISTICS
----------------------------------------
PYTHON -> Highest: 80, Lowest: 80
DDD -> Highest: 75, Lowest: 75
IDA -> Highest: 90, Lowest: 90


Assumptions
Student names are entered correctly by the user.
Grades must be between 0 and 100 inclusive.
Every student must have grades for all three subjects in Section B.
The class contains at least one student.

Limitations
Student names are not checked for duplicates.
Data is stored temporarily in memory only.
Data is lost when the program closes.
Subject names are hardcoded:
PYTHON
DDD
IDA
No file storage or database integration is implemented.

