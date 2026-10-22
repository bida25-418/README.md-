Enter number of students: 2

Input
Student 1
Enter student name: John
Enter PYTHON grade: 75
Enter DDD grade: 80
Enter IDA grade: 70

Student 2
Enter student name: Mary
Enter PYTHON grade: 90
Enter DDD grade: 88
Enter IDA grade: 92

Output

GRADEBOOK SUMMARY
----------------------------------------
John - Average: 75.00
Mary - Average: 90.00

Enter student name to search: Mary

STUDENT DETAILS
----------------------------------------
Name: Mary
PYTHON: 90.0
DDD: 88.0
IDA: 92.0
Average: 90.00



Class Architecture
Class Relationship
+------------------+
|    Gradebook     |
+------------------+
| - students[]     |
+------------------+
| + add_student()  |
| + remove_student()|
| + search_student()|
| + display_all_students()|
+------------------+
          |
          | Contains
          v
+------------------+
|     Student      |
+------------------+
| - name           |
| - grades{}       |
+------------------+
| + add_grade()    |
| + calculate_average()|
| + display_student()  |
+------------------+

Methods:

add_grade() – adds a grade for a subject.
calculate_average() – calculates the student's average mark.
display_student() – displays all student details.

Assumptions and Limitations
Assumptions
Student names are entered correctly.
Subject names are predefined:
PYTHON
DDD
IDA
Grades are entered as numeric values.
Each student has one grade per subject.
Limitations
Student names are case-sensitive.
"John" and "john" are treated as different students.
No input validation is implemented for invalid grades.
Grade ranges are assumed to be between 0 and 100.
Data is stored in memory only.
Student records are lost when the program closes.
Duplicate student names are allowed.
