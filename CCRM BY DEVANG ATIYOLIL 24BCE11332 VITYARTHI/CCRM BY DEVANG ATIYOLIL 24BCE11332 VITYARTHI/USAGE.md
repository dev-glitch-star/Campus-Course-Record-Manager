# CCRM Usage Guide

This application is menu-driven. On startup, you will see the main menu.

## Initial Data
The application attempts to load `students.csv` and `courses.csv` from the `test-data/` folder on startup. Ensure these files are present.

## Main Menu Options

1.  **Student Management:**
    *   Add new students.
    *   List all registered students.
    *   Update a student's email.
    *   Deactivate a student (sets their status to inactive).

2.  **Course Management:**
    *   Add new courses.
    *   List all available courses.
    *   Assign an instructor to a course (instructors are pre-loaded for demo).
    *   Search for courses by instructor, department, or semester.

3.  **Enrollment Management:**
    *   Enroll a student in a course. The system checks for duplicate enrollments and a basic credit limit (15 credits per semester).
    *   Unenroll a student from a course.

4.  **Grade Management:**
    *   Record a grade for a student in an enrolled course.

5.  **View Student Transcript:**
    *   Enter a student's registration number to see their enrolled courses, grades, and calculated GPA.

6.  **Import/Export Data:**
    *   Import student and course data from CSV files in `test-data/`.
    *   Export current student and course data to new CSV files (e.g., `students_exported.csv`, `courses_exported.csv`) in `test-data/`.

7.  **Backup Data & Show Size:**
    *   Performs a backup: Copies all files from `test-data/` to a new timestamped folder within the `backup/` directory.
    *   Shows the total size of all files within the entire `backup/` directory, demonstrating a recursive file traversal.

8.  **Show Java Platform Note:**
    *   Displays a brief explanation of Java SE, ME, and EE.

0.  **Exit:**
    *   Closes the application.

## Sample Interaction

1.  **Run the application.**
    - Initial student and course data will be loaded.
2.  **Enter `1` for Student Management**, then `1` to **Add Student**. Provide details.
3.  **Enter `2` for Course Management**, then `1` to **Add Course**. Provide details.
4.  **Enter `3` for Enrollment Management**, then `1` to **Enroll Student in Course**.
    - Use student registration numbers (e.g., S001) and course codes (e.g., CS101).
5.  **Enter `4` for Grade Management** to record a grade for an enrolled student.
6.  **Enter `5` for View Student Transcript** and enter a student's RegNo to see their academic record and GPA.
7.  **Enter `7` for Backup Data & Show Size.**
    - You will see a new folder created in the `backup/` directory, and then the total size will be displayed.
8.  **Enter `0` to exit.**