# CampusMate - Student Productivity System

## Overview
CampusMate is a command-line Python application for managing common academic tasks in one place. It stores a student profile, assignments, attendance, study sessions and academic performance using SQLite.

## Main Features
1. Student Profile - create and view profile information.
2. Assignment Manager - add, view, update, delete, search, complete and list upcoming assignments.
3. Attendance Manager - calculate attendance, show warnings below 75%, and calculate classes needed to reach 75%.
4. Study Planner - create study sessions, mark them complete, delete them and view study-hours summary.
5. Academic Performance - store marks, calculate totals and grades.
6. Dashboard & Reports - view combined academic status and alerts.

## Technologies
- Python 3
- SQLite
- Python standard library
- unittest
- Git and GitHub

## Requirements
Python 3.10 or later is recommended. No external packages are required.

## How to Run
1. Open a terminal in the project folder.
2. Run `python main.py` on Windows.
3. On systems where `python` points to another version, use `py main.py` or `python3 main.py`.
4. The program automatically creates the `data` folder and `campusmate.db` file.

## How to Test
Run:

`python -m unittest discover -s tests -v`

The test suite checks attendance calculations, performance calculations and input-validation logic.

## Project Structure
- `main.py` - program entry point and main menu
- `src/database.py` - SQLite connection and table creation
- `src/validation.py` - input validation helpers
- `src/student.py` - student profile module
- `src/assignments.py` - assignment module
- `src/attendance.py` - attendance module
- `src/study_planner.py` - study planning module
- `src/performance.py` - academic performance module
- `src/reports.py` - dashboard and alerts
- `tests/` - automated tests

## Important
The project is intended to be customized by the student. Add your own comments, examples, screenshots, and improvements and make sure you can explain every module during evaluation.
