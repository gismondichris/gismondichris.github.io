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
of a data report for sample data. The data must be properly 
formatted and several fields in the report must be populated
values.

#### Description
This is a Python command line program coupled with a VBA macro that allows the users to enter report specific 
values: report date, sampling date, report comments, etc.

Originally this program was designed to generate reports based on a single project. 
More projects were added later and it had to be upgraded to allow the user
to select which report type was being generated. Different report types would accept different 
report specific values. The formatted also varied between report types.

After the user finishes entering information, it reads in the data from a file. 
The data is reformatted as needed and then exported to an excel file.

From there, the VBA macro executes completing some formatting that was not easily achievable in Python.
The VBA macro also exports the excel file to a pdf with modified fields for the official report.