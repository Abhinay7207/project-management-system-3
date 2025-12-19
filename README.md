## How to use Project Management System


## Setup and Run
This is a Java Swing application built with NetBeans.
1. Open the project in Apache NetBeans or any Java IDE.
2. Ensure you have JDK 8 or later installed.
3. Run `src/StartFrame.java` to launch the application.

## How to use Project Management System

**Note**: The system now includes validation to prevent invalid data entry.
- **IDs** must be numeric.
- **Dates** must be in DD/MM/YYYY format.
- **Salaries** and **Budgets** must be positive numbers.

## Project Guidelines
Please refer to the following documents for project requirements and coding standards:
- [Core Feature Implementation](Core%20Feature%20Implementation.md)
- [Error Handling & Robustness](Error%20Handling%20&%20Robustness.md)
- [Integration of Components](Integration%20of%20Components.md)
- [Event Handling & Processing](Event%20Handling%20&%20Processing.md)
- [Data Validation](Data%20Validation.md)
- [Code Quality & Innovation](Code%20Quality%20&%20Innovation.md)
- [Project Documentation](Project%20Documentation.md)
When prompted with the "Enter Your Info" screen, you can use various Administrator or Employee IDs to grant access to the system.

These IDs are provided in the first column of the information listed in "FAdmin.txt" or "FEmployee.txt".

I have provided an example login below for your convenience.


___
### Admin:
Company ID: 11000

Company Password: 312

### Employee:
Company ID: 12006

Company Password: 6
___

When you have successfully logged into the system, select "Show My Info" to display your employee information.

> If you are an administrator, you have the added ability to create employees.

You will be provided with four project processes:
1. Search or Delete Project
2. Add New Employee
3. Create a New Project
4. Company Info



## Search or Delete Project
Here, you can search for a valid Project ID to view its information.

Some of this information includes: Project Name, Due Date, Budget, and Completion.

You may also choose to delete a project on this screen.

## Add New Employee
> Please note that this is an administrator-only feature.

Here, you can enter a new employee's information such as Nane, Age, and Base Salary.

When "ADD" is selected, the employee will be added to FEmployee.txt

## Create a New Project
Here, you can create a new project for your company, as well as add new employees to the project.

Start and due dates must be in the following order: DD/MM/YYYY

When "Add Project" is selected, the project will be added to FProject.txt

## Company Info
Here, you can view various data for the company: Project Info, Administration Info, and Employee Info.

When "DISPLAY" is selected, all information you requested will be provided in list format.

For projects, this includes Project ID, Budget, Expected Profit, and Progress.

For employees/administrators, this includes Name, Job, Age, and Base Salary.
