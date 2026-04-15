## Project Description
This is a simple Python program that records and manages attendance for students and employees. It allows users to add participants, mark them as present, tardy, or absent, and view attendance summaries.
The program also includes the ability to search for participants and displays alerts when someone has been absent too many times. Additional features include time-in recording, tardiness calculation, and recording reasons for absence or tardiness.

## Features
Add and remove participants

Marks attendance for each day

View daily attendance records

Display attendance percentage for each participant

Displays how many times they were absent or tardy

Search participant

Absent warning alert (maximum of 5 absences)

## Features [UPDATED]

Checks whether tardy is excused or unexcused

Checks whether absence is excused or unexcused

Asks the user why the participant is absent or tardy

Records time-in for participants

Calculates and displays the number of minutes late

## How to Run the Program
1. Make sure you have Python installed.
2. Download the file RollCall.py.
3. Open a terminal or command prompt.
4. Run the program:
  python RollCall.py
  or press F5 / click “Run” if using an IDE.
5. Follow the on-screen instructions to manage attendance.


# Example Output
Add participant

Mark attendance

View attendance

Search participant

Remove participant

Exit

Choose an option: 2
Enter name: Alice
Mark as (P/A/T): T
Attendance marked!
Choose an option: 3

--- Attendance Records ---
Alice - P:0 A:0 T:1 | 0.0%


## Contributors
ZAMORA – Attendance marking and counting system
VIDUYA – Data storage and retrieval
LADAGA – User interface and error handling

## Detailed Methodology
  a. Add and Remove Participants
Participants are stored in a structured format:
Each participant is assigned a unique ID
Adding a participant appends their record to the data structure
Removing a participant deletes their record from the system

  b. Mark Attendance
Attendance is recorded daily with three possible statuses:
Present
Tardy
Absent
The program updates attendance by:
Storing daily records in a file
Automatically updating attendance percentages

  c. Attendance Percentage & Summary
Attendance is calculated using the formula:
Attendance = (Days Present / Total Recorded Days) × 100
The system displays:
Name
Total absences
Total tardies
Total days present
Attendance percentage

  d. Search Participant [UPDATED FEATURE]
The user can search for a participant by typing their name to quickly find their record.

  e. Warning of Total Absences
If a participant reaches 5 absences, the program shows a warning message.

# Technologies Used
Python
Suitable for small systems
Provides built-in tools like lists and dictionaries for simple data handling

Back-end: Python code that processes attendance, calculations, and data storage

Front-end: Text-based interface in the command line where users input commands

# Key Designs and Trade-offs
a. Simplicity over Complexity
The system uses text files instead of a database, making it easier to build but less suitable for very large groups

b. Console Interface
The system uses a text-based interface instead of a graphical interface

c. Fixed Absence Limit
The warning is set at 5 absences. This is simple but cannot be changed without editing the code

# Ethical Considerations
a. User Privacy
The program only stores attendance information and does not collect unnecessary personal data

b. Data Safety
Data is stored locally, reducing online risks

c. Accessibility
The system can run on basic computers without requiring high performance

## Commit Messages
Updated the README.md to provide a clearer description of the RollCall project and to include the updated features such as participant search and the absence of warning alert system. 
(egviduya2030 authored) 

Updated the RollCall program code to include a participant search feature and an automatic absence warning system that notfies the user when a participant reaches the maximum absence limit.
(christuffjetlee updated the code)

Updated the README.md to include a detailed methodology explaining how the RollCall system works, covering core feature implementation, attendance calculations, updated search functionality, absence warning logic, technologies used, system design decisions, and ethical considerations.
(zelzamora2030 authored)

Zelmora2030 merged pull request #1 from christuffjetlee/patch-1 to update the RollCall program with the latest improvements.

Updated the README.md to include instructions on how to run the program, added participant search functionality, and implemented an automatic absence warning system for participants who reach the maximum absence limit.
(zelmora2030 authored)

Updated the README.md to improve the arrangements for the Detailed Methodology.
