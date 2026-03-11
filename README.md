# Project Title: RollCall

## Project Description
This is a simple Python program that records and manages attendance for students and employees. It allows adding new participants, marking them as present, tardy or absent,and viewing attendance summaries. The program now includes the ability to search for participants, and shows alerts when someone has been absent too many times.

## Features
- Add and remove participants
- Marks attendance for each day
- View daily attendance records
- Display attendance percentage for each participant
- Displays how many times they were absent or tardy
- Search participant
- Absent warning alert (maximum of 5 absences)

## Features [UPDATED]
-	Checks Whether Tardy is Excused or Unecused
-	Checks Whether Absence is Excused or Unexcused
-	Asks the User why the participant is Absent or Tardy
-	Records Time In for participant
-	Calculate and Display number of minutes late

## How to Run the Program
1. Make sure you have Python installed.
2. Download the file RollCall.py
3. Open a terminal or command prompt.
4. Run the program by pressing F5 or clicking 'Run' 
5. Follow the on-screen instructions to manage attendance.

##Example Output
1. Add participant
2. Mark attendance
3. View attendance
4. Search participant
5. Remove Participant
6. Exit

Choose an option: 2
Enter name: Alice
Mark as (P/A/T): T
Attendance marked!

Choose an option: 3

--- Attendance Records ---
Alice - P:0 A:0 T:1 | 0.0%

## Contributors
- ZAMORA: Name of member 1 (attendance marking and counting system)
- VIDUYA: Name of member 2 (data storage and retrieval)
- LADAGA: Name of member 3 (UI and error handling)


## Detailed Methodology
1. Implementation of Core Features

a. Add and Remove Participants
Participants are stored in a structured format. 
    - each participant is assigned a unique ID.
    - adding a participant appends their record to the data structure.
    - removing a participant deletes their record from the system.

b.  Mark Attendance
Attendance is record daily with three possible statuses:
    * Present
    * Tardy
    * Absent
The program updates the attendance record by:
    - Storing daily records in a file
    - Updating the total attendance percentage automatically.

c. Attendance Percentage & Summary
Attendace = Days Present/Total Recorded Days x 100

The system then displays:
    * Name
    * Total Absences
    * Total Tardies
    * Total Days Present
    * Attendance Percentage
    
d. Search Participant [UPDATED FEATURE]
The user can search a participant by typing their name or a participants name to quickly find their record.

e. Warning of Total Absences
If a participant reaches 5 absences, the program shows a warning message.

2. Technologies Used
    - Python:
        - Good for Small Systems like this
        - Contains built-in tools like lists and dictionaries that makes recording data simple

3.  Back-end & Front-end
    - Back-end: The PYTHON CODE that processes attendance, calculations, and data storage.
    - Front-end: The text shown in the command-line where the user inputs the commands.

4. Key Designs and Trade-offs

a. Simplicity over Complexity
    - The system uses  text files instead of a database, which makes it easier to build. However, it may not handle VERY large groups.

b. Console Interface
    - The system uses text-based interface instead of a graphical one.

c. Fixed Absence Limit
    - The warning is set ay 5 absences. This is simple, but it cannot be changed unless the code is edited.

5. Ethical Considerations
a. User Privacy: The program only stores attendance information. It does not collect unnecessary personal details.

b. Data Safety: The data stored locally, which reduces online risks.

c. Accessibility: The program/system can run on basic computers without needing high performance.

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
