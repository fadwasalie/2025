====================================================
POLICE CASE MANAGEMENT SYSTEM
====================================================

Boston City Campus - Bellville
Student Name: Fadwa Salie
Student Number: 05HA2401762
Module: Systems Development 2A
Assignment: SA1

1. Overview
Police Case Management System is a complete System written in Java based on NetBeans IDE with MySQL database. The system enables the police officers to effectively manage the case records, create new cases, access the case details, and keep a record of the officers using an easy to use Swing GUI.

2. Purpose of the Program
It enables users to administer police officers and police cases in a database.
It has a graphical user interface (GUI) in which a user can use for the following:
• Officer Management: Add, update, delete, and see police officer records.
• Register, update, delete and view criminal case records: This will be enabled through case management.
• Database connection: Complete JDBC connection with MySQL database.
• Exception Handling: Strong exception management in order to avoid crashing of the system.
• User-Friendly Interface: Tabbed intuitively made Swing GUI.

3. System Requirements
• Java Development Kit (JDK) 8 or more.
• NetBeans IDE 8.2 or higher
• MySQL Server 5.7 or higher
• MySQL Workbench

4. Structures and Descriptions of Classes of the Project:
DatabaseConnection.java- This Java and MySQL connexion (through JDBC).
Officer.java- A record Officer (ID, name, rank, phone).
Case.java - Representation of Case record (ID, type, description, etc.).
OfficerDAO.java - Officer database data operations (CRUD).
CaseDAO.java - CLRDAO Handles Case database (CRUD).
PoliceCaseManagementGUI.java The overall user interface including buttons, text field, and table.

4. Installation and Setup
	A) Database Setup
	1. Open MySQL Workbench
	2. Run the database setup SQL script and create:
	- `crime\_management` database
	- Tables necessary ( Officer, Case, CrimeCategory, CaseStatus).
	- Sample data for testing

	B) Java Project Setup
	1. Open NetBeans IDE
	2. Establish a new Java project with the name PoliceCaseManagement.
	3. Place all Java files in the package, which is the src/policecasemanagement:
	- `PoliceCaseManagementGUI.java`
	- `DatabaseConnection.java`
	- `Officer.java`
	- `Case.java`
	- `OfficerDAO.java`
	- `CaseDAO.java`

	C) Database Configuration
	Be sure that MySQL connexion information ( username, password, database name ) in DatabaseConnection.java match your system setup.

	D) MySQL Connector
	Include MySQL JDBC Connector to your project:
	1. Project Properties Right-click project Properties
	2. Libraries \\u2192 Add JAR/Folder
	3. Choose MySQL connector Jar file.

	E) Running the Application
	1. verify server of MySQL is started.
	2. Open the project in NetBeans
	3. execute the Policemanagementgui: PoliceCaseManagementGUI.Java
	4. The main interface will be the opening but-in of the application window.

5. Usage Instructions
	Officer Management Tab
	1. Adding an Officer: Enter your First Name, Last Name, Rank and Phone (optional) and press Add Officer.
	2. Update Officer: Pick an officer in the table, edit the fields, and of course, click on the update officer.
	3. Delete Officer\*\*: Choose an officer in the table and press on Delete Officer.

	Case Management Tab
	1. Add Case Fill in Case Details, Attending Officer ID, Category, Location, Reported Date (yyyy-MM-dd format), and Status (0 Open, 	1 Closed)
	2. Update Case: Choose a case in the table, edit the fields and press the button Update Case.
	3. Delete Case: Choose some case in the table then click on the Delete Case.

6. Sample Data (Question 5)
	This system has the following sample cases:
	1. Burglary City Mall - Under Investigation officer James Patel (2025-05-05)
	2. Cyber Fraud complaint - Officer Lerato (Open, 2025-05-03) - Since this is an instance of free-pressure, location need not be mentioned, but this 	can aid in determining the date of the complaint further.
	3. Officer Dlamini (Under Investigation, 2025-05-01) in case of retrieving a stolen car.
	4. Attack Nightclub - Have Officers Report, Officer Khan Case (Closed, 2025-04-28).
	5. The case concerned a domestic dispute case, involving an officer named Nkosi (Open, 2025-04-30).

7. Error Handling
The system will also have extensive error management on:
Database connection failures: Connection failures may arise from inadequate database maintenance, insufficient scripts and coding, or improperly commercialized database software.<|human|>Database connection failures: Database connection failure may be caused by ineffective database maintenance, inappropriate scripts and code, or commercialisation of database software.
• Invalid date formats
• Missing required fields
• SQL exceptions
• Input validation errors

8. Code Structure
• Model Classes): `Officer.java and Case.java - Data entities.
• Classes Dao, OfficerDAO, CaseDAO: OfficerDAO.java, CaseDAO.java - Database operations.
• UI Class: PoliceCaseManagementGUI.java Mr. User interface and business logic.

9. Troubleshooting
Common Issues
1."No primary method detected": make sure that you are running Policemanagementgui.java file.
2. Connection to the database failed: Connection variables are accurate and MySQL server is operating.
3. "Class not found": Add MySQL connector Jar in project libraries
4. Date formatting error The dates must be in the form yyyy-MM-dd.

10. Dependencies
• Java Swing
• JDBC (MySQL Connector)
• Java AWT
• Java SQL

11. AUTHOR AND DATE
Developed by: Fadwa Salie
Date: 11 November 2025

12. Screenshot
    
    Question 5:
<img width="1225" height="906" alt="Screenshot 2025-11-11 184009" src="https://github.com/user-attachments/assets/041bcb03-a2e0-4a0a-ae75-ae60dc45af17" />

    
