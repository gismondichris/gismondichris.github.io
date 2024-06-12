---
title: Generalized Laboratory Calculation
role:
  - Laboratory Data Manager
languages:
  - VBA
---

#### Summary
Takes in data fields and determines a final concentration for an analyte. 
Can be used to make a variety of calculations for a variety of analytes.

#### Description
This project was driven by the need to mitigate the number of excel 
calculations present in our Laboratory Information Management System (LIMS).
This system allowed users to automatically calculate results using input (database fields) 
and output the results (store them in other database fields). These calculations 
are completed by exporting the input to an excel file, allowing the cells to calculate,
running an optional VBA macro, and then getting the results from certain cells. 
This excel calculation system came with the LIMS.

Over the years, there developed hundreds of excel calculations that had 
been programmed into the LIMS. The sheer breadth of these calculations 
made maintenance difficult. To alleviate this, I created a single excel file and 
macro that could be used to make the majority of the calculations.

The macro takes in several parameters that specify the kinds of calculations that should 
be performed. The macro then analyzes the provided input and performs the relevant 
calculations.

Each individual calculation for this program is trvivial. The real challenge was getting
so many different calculations to feed their input into the same excel sheet, and then 
being able to perform the necessary calculations on it. It required a fair degree of 
abstraction across many different analyses.