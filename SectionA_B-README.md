Gradebook Management System
Project Overview

The Gradebook Management System is a Python application developed for the ICT201 Introduction to Python Programming assignment. The system manages student grades, generates reports for academic performance tracking and demonstrates the use of dictionaries and nested dictionaries for storing and managing student academic records.

This implementation covers:

Section A: Scalar Objects and Loops
Section B: Lists and Tuples
Section C: Dictionaries

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

Section C
Student Record Management
◾ Add multiple student records

◾ Store student data using nested dictionaries

◾ Record grades for:

PYTHON
DDD
IDA

◾ Calculate student averages

Update Operations

◾ Update grades for an existing student

◾ Modify all subject grades

◾ Confirm successful updates

Delete Operations

◾ Remove student records

◾ Confirm successful deletion

Search Operations

◾ Search for a student by name

◾ Display complete student information

◾ Display calculated average

Reporting Features

◾ Display all student records

◾ Display subject-specific grades

◾ Show all PYTHON grades

◾ Show all DDD grades

◾ Show all IDA grades

◾ Generate formatted reports

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

Section B Data Structure

students = {
    "John": {
        "PYTHON": 85,
        "DDD": 78,
        "IDA": 92
    },

    "Mary": {
        "PYTHON": 90,
        "DDD": 88,
        "IDA": 95
    }
}


Input:

Enter number of students: 2

Student 1
Enter student name: John
Enter grade (0-100): 80

Student 2
Enter student name: Mary
Enter grade (0-100): 90

Output:

CLASS REPORT
----------------------------------------
Total Grades : 170.00
Average Grade: 85.00

Student: John Subject: PYTHON Grade: 80.00 Class Average: 85.00
Student: Mary Subject: PYTHON Grade: 90.00 Class Average: 85.00

Multiple Subject

Input:

Student 1
Enter student name: John

Enter PYTHON grade (0-100): 80
Enter DDD grade (0-100): 75
Enter IDA grade (0-100): 90

Output:

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

Input:

Enter number of students: 2

Student 1
Enter student name: John
Enter PYTHON grade: 80
Enter DDD grade: 75
Enter IDA grade: 90

Student 2
Enter student name: Mary
Enter PYTHON grade: 92
Enter DDD grade: 85
Enter IDA grade: 88

Output:

STUDENT RECORDS
----------------------------------------

Name: John | PYTHON: 80.0 | DDD: 75.0 | IDA: 90.0 | Average: 81.67

Name: Mary | PYTHON: 92.0 | DDD: 85.0 | IDA: 88.0 | Average: 88.33

Update:

Enter student name to update: John

Enter new PYTHON grade: 85
Enter new DDD grade: 80
Enter new IDA grade: 95

Output: 

Student updated successfully.

Remove Example

Input:

Plain Text
Enter student name to remove: Mary

Output:

Plain Text
Student removed successfully.
Search Example

Input:

Plain Text
Enter student name to search: John

Output:

Plain Text
STUDENT FOUND
----------------------------------------
Name: John
PYTHON: 85
DDD: 80
IDA: 95
Average: 86.67


Assumptions
Student names are entered correctly by the user.
Grades must be between 0 and 100 inclusive.
Every student must have grades for all three subjects in Section B.
The class contains at least one student.
Student names are entered correctly.
Grades are numeric values.
Every student has grades for all three subjects.
Student names are unique.

Limitations
Student names are not checked for duplicates.
Data is stored temporarily in memory only.
Data is lost when the program closes.
Subject names are hardcoded:
PYTHON
DDD
IDA
No file storage or database integration is implemented.

