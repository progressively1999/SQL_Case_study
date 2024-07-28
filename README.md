Project Overview
This repository contains SQL scripts to create and manage a database for tracking programmer information, software development, and educational background.

Database Schema
programmer

pname: Programmer's name (Primary Key)
dob: Date of birth
doj: Date of joining
gender: Gender (M/F)
prof1: Primary profession
prof2: Secondary profession
salary: Salary
software

pname: Programmer's name (Foreign Key referencing programmer.pname)
title: Software title
developin: Development language
scost: Software cost
dcost: Development cost
sold: Number of copies sold
studies

pname: Programmer's name (Primary Key and Foreign Key referencing programmer.pname)
institute: Name of institute
course: Course name
coursefee: Course fee
Relationships
A programmer can develop multiple software.
A programmer has only one educational record.
Data Integrity
On deleting a programmer, all associated software and study records will be deleted (ON DELETE CASCADE).
Usage
Create the database and tables using the provided SQL scripts.
Populate the tables with programmer, software, and study data.
Perform queries and analysis based on the stored data.
Notes
Consider adding indexes to frequently queried columns for performance optimization.
Implement data validation and error handling for data integrity.
Explore additional columns or tables to store more detailed information if required.
