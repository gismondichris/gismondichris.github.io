---
title: Customer Data Report
roles:
  - Laboratory Data Manager
  - Laboratory Manager
languages:
  - Python
  - VBA
tools:
  - Git
---

#### Summary
Creates a pdf official copy and an xlsx unofficial copy 
of a data report for sample data. Several fields differ 
between the official and unofficial report. Cells must 
be formatted to properly display data.

#### Description
This is a Python command line program coupled with a VBA macro that allows the users to enter report specific 
values: report date, sampling date, report comments, etc.

Originally, this program was designed to generate reports based on a single project. 
More projects were added later and it had to be upgraded to allow the user
to select the report type. The report type could change the following features:
- Which user specified values were available for user input
- Report formatting
- Data values in certain fields (address, report name, etc.)

After the user finishes entering the user specified values, it reads in the sample data from a file. 
The sample data is reformatted as needed and then exported to an excel file.

From there, the VBA macro executes completing some formatting that was not easily achievable in Python.
The VBA macro also exports the excel file to a pdf with modified fields for the official report.