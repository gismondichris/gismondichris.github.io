---
title: Sample Guarantee Analyzer
roles:
  - Laboratory Manager
languages:
  - Python
---

#### Summary
A Python GUI Windows desktop application where users can enter in
the chemical guarantees of a fertilizer sample. The program then 
displays what analyses to order for the sample. The rules that govern
what analyses to order are governed by a locally stored csv file that 
users can edit to account for changing rules.

#### Description
This was an early project that I developed to save time and increase accuracy 
in the laboratory. The normal process for sample login involves a person
reading the fertilizer guarantees (similiar to nutrition facts on food) and 
determining what anlayses to order based on the guarantees.

However, the rules that govern which analyses to order are not always intuitive. 
The rules also change depending on the labs capabilities at the time. As a result,
there were often corrections that had to be made to the analyses that were ordered.

This application allowed the user to simply enter the guarantees and select
options (based on sources, etc.). The program would then display the correct 
analyses to order based on the rules. I used 
[tkinter](https://docs.python.org/3/library/tkinter.html) to build the GUI.

The creation of the user based rules was the most difficult part of this project.
The rules had to allow for:
- rules based on values: greater, less than, equal to, between, not equal to
- rules based on conditions: does it contain source x
- rules based on multiple values and/or conditions
- cascading rules: if this condition met do rule 1, else continue

These rules would have been trivial to hard code into the program. But one of 
the requirements for the project was that the rules be editable in a csv or excel 
file. As such I had to create an file which allowed the user to enter rules that met
the conditions above.

If I could revisit this project now, I would update the GUI and change the way rules are stored.
An ideal improvement would be to allow users to edit and view rules directly through the GUI. 
But as with many of the projects I completed for the lab, it was more important to 
have minimally viable product available then spend weeks or months perfecting something.

As with many things in life, I learned that its important in software to not let the 
perfect become the enemey of the good.