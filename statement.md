# CampusMate - Problem Statement and Scope

## Problem Statement
Students often manage assignments, attendance, study schedules and marks using separate notes or applications. This makes it harder to track academic tasks and identify important issues such as pending assignments or attendance below the required level.

## Proposed Solution
CampusMate is a command-line Python system that combines these academic activities into one application. It stores data in SQLite and provides menus for managing academic information.

## Target Users
The primary target user is a college student who wants a simple academic management tool that can be run from a computer terminal.

## Scope
The current version covers:
- student profile management
- assignment CRUD and search
- attendance tracking and percentage calculation
- attendance target calculation for 75%
- study session planning
- marks and grade calculation
- dashboard and alerts
- automated unit tests

## Functional Requirements
- The user shall create and view a student profile.
- The user shall add, view, update, delete and search assignments.
- The user shall record attendance and calculate percentages.
- The user shall create and manage study sessions.
- The user shall record marks and calculate total and grade.
- The system shall show a combined dashboard with alerts.

## Non-Functional Requirements
- Usability: clear menu-driven command-line interface.
- Reliability: validation prevents many invalid inputs.
- Maintainability: code is divided into modules.
- Data persistence: SQLite keeps data after the program closes.
- Error handling: invalid values are rejected and useful messages are displayed.
- Resource efficiency: the application uses a lightweight local SQLite database and standard-library modules.

## Future Enhancements
- login and multiple student profiles
- CSV export
- graphical user interface
- reminder notifications
- cloud synchronization
