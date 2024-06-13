---
title: VBA
projects:
  - Customer Data Report
  - Feed Report Macro
  - Automatic Form Completion
  - Generalized Laboratory Calculation
roles:
  - Laboratory Data Manager
  - Laboratory Manager
  - Analytical Chemist
---

I have used VBA primarily for calculations, data formattiing, 
and report generation.

The Laboratory Information Management System (LIMS) I managed
used Excel to perform calculations, with specified database fields 
as input and output. The input fields are loaded into specified cells,
the sheet is allowed to calculate, and the output fields are taken 
from specified fields. The LIMS also allowed the user to call macros.
This allowed for much more complicated calculations. I would 
often use VBA to perform calculations that would otherwise be tedious to 
compose use Excel formulas alone.

I would also use VBA to generate reports and/or forms. This process was 
sometimes coupled with a Python application to handle some of the 
more abstract parts of the program logic. The reports would be exported from 
an Excel template to a .pdf final version of the report using VBA. The report 
generation often involved performing data clean-up such as converting
value of "0" to "Not detected" and formatting cells to show the proper 
number of [signifigant figures](https://en.wikipedia.org/wiki/Significant_figures) for values.

Data formatting was another common task that I achieved utilizing VBA.
The data taken from instruments was often in a format  incompatible with 
out data upload software for the LIMS. Since these output files were often .csv 
or .xlsx, it was trivial to write VBA applications to rearrange columns, format dates, 
replace values, etc. This allowed lab personnel to avoid doing such tasks manually.