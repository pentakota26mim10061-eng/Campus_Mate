## CampusMate – Student Productivity System

## 1. Introduction

CampusMate is a simple command-line application developed in Python to help college students manage their academic

activities from one place.

Students normally keep track of assignments, attendance, study plans, and marks separately. This can make it difficult to get a quick idea of pending work or academic progress. CampusMate combines these activities into one menu-driven

application and stores the information locally using SQLite.

The project was developed as an academic project for the Introduction to Problem Solving and Programming (CSE

1021) course.

- 2. Objectives

The main objectives of CampusMate are:

- To maintain basic student profile information.

- To keep track of assignments and their status.

- To calculate and monitor attendance.

- To plan and record study sessions.

- To store marks and calculate academic performance.

- To provide a dashboard containing important academic information.

- To save data locally so that it is available when the program is opened again.

- To use input validation and error handling to avoid common invalid entries.

## 3. Features

## Student Profile

The Student Profile section allows the user to create and view basic profile information.

## Assignment Manager

The Assignment Manager provides options to:


- Add assignments

- View assignments

- Update assignments

- Delete assignments

- Search assignments

- Mark assignments as completed

- View upcoming assignments

## Attendance Manager

The Attendance Manager can:

- Record attendance Calculate attendance percentage Display a warning when attendance is below 75%

- Calculate the number of additional classes required to reach 75%

## Study Planner

The Study Planner allows the user to:

- Create study sessions

- View and manage study sessions

- Mark sessions as completed

- Delete sessions

- View a summary of study hours

## Academic Performance

This section is used to:

- Store marks

- Calculate totals

- Calculate grades

- Keep academic performance information in one place

## Dashboard & Reports

The dashboard combines information from the different modules and displays an overall academic status with useful

alerts.

## 4. Technologies Used

The project uses the following technologies:


- Python 3 – main programming language

- SQLite – local database

- Python Standard Library – built-in Python modules

- unittest – automated testing

- Git and GitHub – source code management and project submission

No external Python packages are required for the current version.

## 5. Requirements

Before running the project, make sure Python is installed.

## Recommended version

Python 3.10 or later

To check the installed Python version:

python --version

On some Windows systems, the following command can also be used:

py --version

No additional package installation is required.

## 6. Project Structure

The project is organized into separate files so that each part of the application has a specific responsibility.


File

main.py

src/database.py

src/validation.py

src/student.py

src/assignments.py

src/attendance.py

## Important files

Purpose

Starts the application and displays the main menu

Handles SQLite connection and database setup

Contains input validation functions

Handles student profile operations

Handles assignment management

Handles attendance calculations

src/study_planner.py Handles study sessions

src/performance.py

src/reports.py

tests/

requirements.txt

README.md

The data folder and database file are created automatically when the application initializes the database.

Handles marks and grades

Generates dashboard information and alerts

Contains automated tests

Lists project dependencies

Project documentation


## Step 1 – Open the project folder

Open Command Prompt or PowerShell and move to the CampusMate project folder.

For example:

cd path o\CampusMate

## Step 2 – Check Python

Run:

python --version

## Step 3 – Start the application

Run:

python main.py

If python does not work on Windows, try:

py main.py

On systems where Python is available through python3, use:

python3 main.py

## Step 4 – Use the main menu

After starting the program, the CampusMate menu is displayed.

The main options are:


1. Student Profile 2. Assignment Manager 3. Attendance Manager 4. Study Planner 5. Academic Performance 6. Dashboard & Reports

7. Exit

Select the required option and follow the instructions shown in the terminal.

## 8. Database

CampusMate uses SQLite for local data storage.

The database is created automatically by the application. It does not require a separate database server.

The database is stored as:

data/campusmate.db

This allows information entered by the user to remain available after the program is closed and opened again.

## 9. Input Validation

Input validation is included to handle common incorrect entries.

For example, the program checks values entered for different academic operations and displays a message when an

invalid value is entered instead of allowing the program to continue with incorrect data.

The validation functions are kept separately in:

src/validation.py

This keeps validation logic separate from the main feature modules.

## 10. Testing

The project includes automated tests using Python's built-in unittest framework.

To run all available tests:


python -m unittest discover -s tests -v

The tests cover important parts of the application such as:

- Attendance calculations

- Academic performance calculations

- Input validation

No external testing package is required.

## 11. Typical User Flow

A typical use of CampusMate can be:

2. Create or view the student profile.

3. Add current assignments.

4. Update assignments as work progresses.

5. Enter attendance information.

6. Check the attendance percentage.

7. Add study sessions to the study planner.

8. Enter academic marks.

9. Open the dashboard to review the overall academic information.

10. Exit the application.

The information is stored locally in the SQLite database.

1. Start the application.

## 12. Error Handling

The application is designed to handle invalid inputs and common user mistakes without unnecessarily terminating the

program.

Validation is used before important values are processed. This helps maintain correct information in the database and

gives the user an opportunity to enter the value again.

## 13. Design Approach

CampusMate follows a modular design.


Instead of keeping the entire program in one Python file, different responsibilities are divided into separate modules. For example, attendance-related operations are handled by the attendance module, while assignment operations are

handled by the assignment module.

This approach makes the project easier to understand, test, and modify.

The main program acts as the entry point and connects the different modules through the menu.

## 14. Limitations

The current version is designed as a local command-line application. Some features that are not included in the current

version are:

- Multiple user accounts

- Online/cloud synchronization

- Mobile application support

- Graphical user interface

- Automatic notification services

- Online access to academic data

These can be considered for future versions.

## 15. Future Enhancements

Possible improvements for future versions include:

1. Adding login support for multiple students. 2. Adding a graphical user interface. 3. Adding export of academic data to CSV files. 4. Adding reminders for assignments and study sessions. 5. Adding charts for attendance and academic performance. 6. Adding cloud synchronization. 7. Adding notification support for important deadlines.

## 16. Conclusion

CampusMate brings several common academic activities into a single application. It provides a simple way to manage

assignments, attendance, study sessions, marks, and academic reports from a computer terminal.

The project demonstrates the use of Python programming, functions, modular programming, file and database handling, input validation, exception handling, and automated testing. SQLite provides local data persistence without requiring a

separate database server.


The current version focuses on keeping the application simple and practical while providing a foundation for adding more

features in the future.

## 17. Author

## Course: 

Student Name: Pentakota Hemanth 

Registration Number: 26MIM10061 

College: VIT Bhopal 

Academic Year: 2026–2027

## 18. License

This project was developed for academic and educational purposes.
