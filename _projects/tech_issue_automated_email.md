---
title: Tech Issue Automated Email
roles:
  - Laboratory Data Manager
tools:
  - Power Automate 
---

#### Summary
Information regarding tech issues is sent to the 
Laboratory Data Manager (myself) and a notification email 
is sent to the user who submitted the issue.

#### Description
This is a simple Power Automate Flow that triggers on the completion
of a Microsoft Form. The data from the form is exctracted and sent 
in an email to the Laboratory Data Manager. A notification email is 
sent to the user. 

If a user responds to the email, it is automatically sent to the 
relevant party. That is, the user who submitted would respond to 
the Laboratory Data Manager. The Laboratory Data Manager would 
respond to the user who submitted the issue or request.

This project was implemented to address the lack of ticketing 
system within our section. A button was added to out Laboratory 
Information Management System that would take users directly to the 
Microsot Form.