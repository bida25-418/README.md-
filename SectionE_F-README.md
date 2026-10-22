Gradebook Management System - Sections E & F 
Project Overview

The Gradebook Management System for Sections E and F demonstrates the use of Object-Oriented Programming (OOP) and Exception Handling in Python.

The system is designed to manage student records, store grades, calculate averages, search for students, sort records, and handle invalid user input through custom exceptions.

Section E 
Classes and Objects
Constructors (__init__)
Methods
Encapsulation
Object interaction

Section F 
Custom Exceptions
Input Validation
Error Handling
Searching and Sorting Algorithms
Enhanced Gradebook Management

Features List
Section E 

◾ Create student objects

◾ Store grades using dictionaries

◾ Calculate student averages

◾ Display student details

◾ Add students to a gradebook

◾ Search for students by name

◾ Display gradebook summaries

◾ Object-oriented implementation


Section F 

◾ Custom exception handling

◾ Grade validation (0-100)

◾ Duplicate student detection

◾ Student search with exceptions

◾ Sort students alphabetically

◾ Sort students by average grade

◾ Error messages for invalid grades

◾ Error messages for non-numeric input

◾ Report generation


Program Architecture

Data Structure Design

Student Object
Student
│
├── name
└── grades
    │
    ├── PYTHON
    ├── DDD
    └── IDA

    Student(
    name="Theo",
    grades={
        "PYTHON": 80,
        "DDD": 75,
        "IDA": 90
    }
)

Gradebook Object

Gradebook
│
└── students
     │
     ├── Student 1
     ├── Student 2
     └── Student n
     
Input

Enter number of students: 2
 
Student 1
Enter student name: Theo
Enter PYTHON grade: 80
Enter DDD grade: 75
Enter IDA grade: 90
 
Student 2
Enter student name: Mpho
Enter PYTHON grade: 95
Enter DDD grade: 88
Enter IDA grade: 92
Gradebook Summary Output
Plain Text
GRADEBOOK SUMMARY
----------------------------------------
 
Theo - Average: 81.67
Mpho - Average: 91.67
Student Search Output

Input:

Plain Text
Enter student name to search: John

Output:


STUDENT DETAILS
----------------------------------------
Name: Theo
PYTHON: 80
DDD: 75
IDA: 90
Average: 81.67
Sorting Functionality (Section F)
Sort by Name

Before Sorting:

Plain Text
Mpho
Theo
Lee

After Sorting:

Plain Text
Theo
Mpho
Lee
Sort by Average Grade

Before Sorting:

Plain Text
Lee 81.67
Mpho 91.67
Theo 75.00

After Sorting:

Plain Text
Theo 75.00
Lee 81.67
Mpho 91.67
Average Grade Formula

The student's average grade is calculated using:

Python
sum(self.grades.values()) / len(self.grades)

Example:

Plain Text
PYTHON = 90
DDD = 80
IDA = 85
 

Calculation:

Plain Text
(90 + 80 + 85) / 3
 
Average = 85.00
Error Handling Examples
Invalid Grade

Input:

Plain Text
Enter PYTHON grade: 120

Output:

Plain Text
Grade must be between 0 and 100.
Non-Numeric Grade

Input:

Plain Text
Enter PYTHON grade: abc
 

Output:

Plain Text
Grades must be numeric.
Student Not Found

Input:

Plain Text
Enter student name to search: Lee

Output:

Plain Text
Student not found.
Duplicate Student Name

Input:

Plain Text
Enter student name: Theo

If a student called Theo already exists:

Plain Text
Duplicate student name.

Assumptions
Student names are entered correctly.
Every student has grades for all subjects.
Users provide the required number of records.
Subject names remain fixed.


Limitations
Data is not saved permanently.
Bubble Sort is inefficient for very large datasets.
No graphical user interface.
Student IDs are not implemented.
Maximum grade validation is limited to 100.
Sorting by average is in ascending order only.
Future Improvements

Potential improvements include:

File storage using CSV or JSON
Database integration
GUI implementation using Tkinter
Student ID management
Additional subjects
Report exporting
Password-protected access
Statistics dashboard
Highest and lowest performer reports
Automatic grade classification

