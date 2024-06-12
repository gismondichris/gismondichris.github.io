---
title: Backlog Generator
layout: tagged_page
languages:
  - Python
tools:
  - Git
roles:
 - Laboratory Data Manager
 - Laboratory Manager
---

#### Summary
The backlog generator is a Python program that generated a pdf backlog of all the samples 
and their current status. The status proved difficult to determine 
as it was not based on any given database field. In addition, object 
oriented design was absolutely critical in maintaining a functional 
and readable program.


#### Complexity
The program itself was not terribly complicated. The data was loaded in and assigned to 
the relevant objects. From there, the objects handled data validation and data processing.
The real challenge was designing the user parameters to determine the sample status, 
especially given that the database itself could not be added to or modified in any way.


#### Requirements
Create a backlog that shows that status 
of all samples in the laboratory.
- The database could not be modified in any way
- All user editable parameters must be stored in csv files
- The status of the sample must be determined using these user parameters\


#### Description
Because there was no field in the database that could be used to determine the 
status of the sample, I designed user parameters that allowed the user to define 
what fields were associated with a given status. In other words, for a given status, the 
user could define:
- the database fields to examine
- the values in those fields that qualified as complete or incomplete

I also created additional user parameters to map the sample status across a variety of 
processes that the sample could be subject to.

A sample consists of processes, which consists of stages. which consists of components.
Each component correlates to a database field.

Then the program would look at the components to determine if a stage was pending previous 
stages, pending with all previous stages complete, in progress, or complete.

Each stage could be assigned a department, which represents groups of people 
in the lab that were responsible for completing that stage.

The reports were organized by department. This was each department could see 
what stages needed to be completed for each sample. They could also see samples that 
were in progress, waiting on previous stages, or even complete. The reports also 
calculated how many days the sample had been waiting for a given stage to complete.

The user defined parameters (such as processes, stages, and departments) were defined 
in the locally stored csv files.

The program was written entirely in Python. The general outline of the program was as 
follows:
- The user defined parameters are loaded in from the locally stored csv's
- The parameter data is validated to ensure there were no conflicts across the files
- The sample data is loaded into memory
- Component data is assigned
- Stages and processes are added based on the components present
- The status of each stage is determined
- The data is formatted in a table
- This table is output to a pdf with color highlighting rules as specified in the user parameters

All in all, there were about 1500 components mapped to about 25 stages across 20+ processes.
