# Medical-Test-Manager
## Description of Bash Script (Patient Record Management System)
This Bash script manages patient medical records by providing functionalities to add, search, update, and analyze medical test results. It uses two files for data storage:

medicalRecord.txt: Stores patient test records.
medicalTest.txt: Contains medical test details (test names, normal ranges, and units).
Core Functionalities:
Add New Medical Test (add_new_test):

Prompts user input for patient ID, test type, date, result, and status.
Validates input formats (7-digit IDs, YYYY-MM dates, numeric test results).
Retrieves units from medicalTest.txt based on the selected test.
Appends validated records to medicalRecord.txt.
Search Tests by Patient ID (search_by_id):

Provides options for searching records by:
All tests for a patient.
Abnormal test results based on predefined ranges.
Tests within a specific date range.
Tests by status (Completed, Reviewed, Pending).
Displays matched records clearly.
Search for Normalized Test Results (search_normalized_tests):

Iterates through all records.
Checks if test results fall within normal ranges specified in medicalTest.txt.
Displays only records with normal test results for each test type (e.g., Hgb, BGT, LDL, systole, diastole).
Calculate Average Test Values (avreg_test_value):

Computes average values for each test type recorded in medicalRecord.txt.
Uses associative arrays to sum and count test results.
Outputs clearly formatted average values.
Update Existing Test Results (update_test_result):

Allows users to update existing records.
Validates patient ID, test name, new result, date, and status inputs.
Updates the specific test entry in medicalRecord.txt.
Menu-driven Interface:
The script continuously presents a menu to the user to easily select and execute desired functionalities:

Add New Test Record
Search Test by Patient ID
Search for Normal Tests
Calculate Average Test Values
Update an Existing Test Result
Exit
Validation and Error Handling:
Robust validation for user inputs (ID, date, result formats).
Error messages guide the user clearly to correct invalid inputs.
Overall, this script provides a comprehensive, interactive system for managing patient medical data effectively from the command line.
