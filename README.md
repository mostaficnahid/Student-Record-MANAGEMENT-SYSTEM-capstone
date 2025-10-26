Student Record Management System (C Language)

A comprehensive, console-based application designed to manage student academic records, personal details, and grades. This project was developed entirely in the C programming language as a capstone to demonstrate proficiency in data management, file handling, and structured programming.

Table of Contents

Project Overview

Key Features

Technologies & Core Concepts

System Requirements

How to Compile and Run

How to Use the System

File Structure

Potential Future Enhancements

Author

Project Overview

This Student Record Management System is a command-line interface (CLI) application that simulates the core data management tasks of an educational institution. It provides a simple, menu-driven workflow for administrators or teachers to perform CRUD (Create, Read, Update, Delete) operations on student records.

All student data (such as roll number, name, class, and marks) is stored persistently in local binary files, which function as a simple, file-based database. This project serves as a practical demonstration of C's capabilities for building robust, data-centric console applications for academic and administrative needs.

Key Features

Add New Student:

Register a new student with essential details like Roll Number, Full Name, Class/Grade, and Contact Information.

Display All Students:

View a neatly formatted list of all student records currently stored in the system.

Search for a Student:

Quickly find a specific student's record by entering their unique Roll Number or Name.

Update Student Record:

Modify the details of an existing student (e.g., update contact info, or class).

Delete Student Record:

Permanently remove a student's record from the system.

Grade/Mark Management:

Add/Modify Marks: Input or update marks for various subjects for a specific student.

Calculate Results: Automatically calculate the total marks, percentage, and pass/fail grade based on the entered marks.

Persistent Data Storage:

All student records are saved to a file (students.dat), ensuring that data is not lost when the application is closed and reopened.

Technologies & Core Concepts

Programming Language: C (Standard C99)

Compiler: GCC (GNU Compiler Collection) or any other standard C compiler.

Core C Concepts Implemented:

File I/O: Extensive use of fopen, fread, fwrite, fseek, and fclose for persistent data storage in binary files.

Data Structures: Heavy reliance on struct to model the Student entity (containing fields for roll number, name, marks, etc.).

Pointers & Memory Management: Efficient data handling, argument passing, and manipulation using pointers.

Modular Programming: Separation of concerns into functions for each distinct task (e.g., add_student(), search_student(), calculate_grade()).

Standard Libraries: stdio.h, stdlib.h, string.h.

System Requirements

To compile and run this project, you will need a C compiler installed on your system.

Linux: GCC is often pre-installed. (Install with sudo apt-get install gcc).

macOS: Install Xcode Command Line Tools (xcode-select --install).

Windows: Install a C compiler environment like MinGW or use an IDE (Visual Studio, Code::Blocks) with a built-in compiler.

How to Compile and Run

Get the Source Code:
Download or clone the project files to your local machine.

Navigate to the Project Directory:
Open a terminal or command prompt and use the cd command.

cd /path/to/Student-Record-Management-System


Compile the Code:
Use gcc (or your compiler) to create an executable file.

gcc main.c -o student_system


(Replace main.c if your primary source file is named differently. If you have multiple .c files, compile them together: gcc main.c student.c -o student_system)

Run the Application:
Execute the compiled program to start the system.

On Linux/macOS:

./student_system


On Windows:

student_system.exe


How to Use the System

Upon launching the application, you will be presented with a clear, numbered main menu.

=======================================
   STUDENT RECORD MANAGEMENT SYSTEM
=======================================
[1] Add New Student Record
[2] View All Student Records
[3] Search for a Student
[4] Update a Student Record
[5] Delete a Student Record
[6] Add/Modify Student Marks
[0] Exit Application
=======================================
Enter your choice:


Enter the number corresponding to the desired menu option and press Enter.

The system will guide you through all necessary prompts to complete the task.

File Structure

The project is organized with a clean and understandable structure:

.
├── main.c              # The main C source code (handles menus and app flow).
├── students.dat        # Binary file for storing all student records (created on first run).
└── README.md           # This documentation file.


(Optionally, you may have .h files or separate .c files like student.c)

Potential Future Enhancements

This project provides a strong foundation that can be expanded with more advanced features:

Admin Login: Add a password-protected login screen for administrators.

Sorting Records: Implement functionality to sort and display students by Roll Number, Name, or Percentage.

Class-wise Reports: Generate reports showing all students in a specific class or grade.

Attendance Tracking: Add a module for logging student attendance.

GUI: Develop a simple graphical user interface using a library like GTK or Qt.

Author

Author Your Name: Mostafic Yellahy Nahid

GitHub: mostaficnahid

LinkedIn: https://www.linkedin.com/in/mostafic-yellahy-nahid-46a0202b5/
