---
title: Batch Worksheet
roles:
  - Laboratory Data Manager
tools:
  - Crystal Reports
---

#### Summary
Creates a report that list samples and some
of the data related to samples for each of 
75 different methods.

#### Description
The Laboratory Information Management System (LIMS)
had the ability to batch sample analyses. Each batch 
could be linked to a batch report to display information about 
the batch. Because of the way the LIMS was implemented, all
the logic regarding the report had to be done using the Crystal Syntax.
That is, none of the logic could be completed by some other programming 
language.

There were about 75 methods for which reports needed to be generated.
Each report needed to access different database items and fields
depending on the method being reported on. However, the report 
would be formatted the same. Thus, a change to one report 
would need to be duplicated across all 75 reports.

Rather than create 75 reports with slight variation, I created one 
report and used a combination of shared variables, functions, and 
subreports to gather the relevant data. 

This proved challenging as
there are limitations in the Crystal Syntax. You can not have a subreport within a subreport.
You also can not have an array of arrays. This forced me to think
critically about how to structure and access data during the execution.
