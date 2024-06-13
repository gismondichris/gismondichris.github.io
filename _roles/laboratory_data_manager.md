---
title: Laboratory Data Manager
projects:
  - Database Updates
  - Backlog Generator
  - Customer Data Report
  - Discard List Report
  - Automatic Form Completion
  - Generalized Laboratory Calculation
  - Tech Issue Automated Email
  - Database ERD Design
  - Batch Worksheet
  - General Crystal Reports
  - Automatic Network Drive Connection
languages:
  - Python
  - VBA
  - SQL
tools:
  - Crystal Reports
  - Git
  - Oracle SQL Developer
  - Power Automate
  - PowerShell
---

#### Summary
My role here was to manage all of the data and 
data systems in the laboratory. This role gave me more 
technological experience than any other role I have had.
Some of my repsonsibilities in this role included coordinating
all tech issues, 
building reports, automating tasks, and coordintating tech projects.

#### Positions 
I performed this role as part of my Chemist Specialist (2022-present), 
Environmental Specialist III (2020-2022), and Chemist Administrator (2018-2020)
positions.

#### Automating Tasks 
Much of my role consisted of looking for ways to automate tasks. Sometimes 
these automations were quite simple, such as creating a 
[VBA macro]((% link _projects/file_conversion.md %)) to reformat data in 
a file. Other times, this involved more extensive programming. For example, 
I created a combined [Python and VBA application]({% link _projects/customer_data_report.md %}) to create reports for 
the water nutrients prgram. This application had to allow the user 
to specify a number of different parameters depending on the report 
type that was being generated. All in all, this application took about 1-2 minutes to run. 
The original task usually took 1-2 hours to manually do all the formatting.

Another example of automation is creating a 
[ticketing system]({% link _projects/tech_issue_automated_email.md %}) for users to submit 
issues they are having and integrating this into our existing LIMS application.

#### Maintaining Laboratory Information Management System (LIMS)
The laboratory utilized a LIMS provided by [Labworks](https://labworks.com/). I was 
responsible for maintaining this system.

The system consists of a user desktop GUI and a database backend. The database was managed 
by our IT department. I managed everything from the user side. This including managing 
user created analyses (10k+), calcuations for data (500+), reports (75+), and many 
other features. As part of handling the calculations, I wrote several VBA macros 
to streamline and simplify maintenance (example [here]({% link _projects/generalized_laboratory_calculation.md %})).

Since I handled any issues related to the application, I frequently encounterd issues 
with our database structure. This was a typically result of custom software that had been 
created in the early 2000's and did not allow us to run the automatic update tool 
provided by the vendor. In any case, I would use [Oracle SQL Developer]({% link _tools/oracle_sql_developer.md %})
to examine the database and write [SQL scripts]({% link _projects/database_updates.md %})
 to address any issues I found. This often 
involved coordinating with the IT team and the vendor to ensure all changes were correct.

#### Maintaining Document Control Software
For a time, I was responsible for maintaining our Document Control Software 
provided through [Paradigm](https://www.paradigm3.com.au/compliance-management-software-package-paradigm-3/).
This program handled document version control, deviations, non-conformances, and other quality assurance 
related documentation. Part of managing this application included leading 
monthly document review meetings with management.
The software is relatively simple and straightfoward to use. The main 
tasks associated with this application were:
- Tracking the state of every document 
- Ensuring every document met quality standards
- Working with lab personnel to move documents through the review process
- Adding/removing users
- Assigning permissions/roles
- Troubleshooting any issues

#### Building Reports
I built reports for subjects such as data review, data reporting, and sample status.
These reports were built using Python, VBA, and Crystal reports. In most cases,
the reports were built in response to the developing needs of the laboratory.
Simple reports just queried the database and displayed the results. Complex 
reports sometimes required months of planning and work (example [here](% link _projects/backlog_generator.md %))

The reports also had to be maintained. Careful attention was required 
when changing any portion of the LIMS, as this may inadvertently affect the reports 
if they queried related fields.

#### Project Management
I was responsible for driving all out tech projects foward and knowing 
that status for any given project at all times.

Some of the projects were individual projects and others 
were completed almost entirely by others. There were two major components 
to this work. First, I had to maintain documentation of the status of 
all my projects. If the project was simple, this may be as small as 
a few lines of text. But often, this consisted of a timetable 
which showed all work that had been done, is currently being done, and what 
the current plan is.

I initiated a monthly meeting to review the status of all tech projects and 
issues with the management team. This helped steamline communication and 
aided in making adjustments to the laboratory's developing needs.
