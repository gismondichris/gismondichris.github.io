---
title: Python TCP Server
languages:
  - Python
  - SQL
  - Java
  - Git
---

#### Summary
An educational project that featured a Java GUI front-end and 
a Python back-end.

#### Description
The back-end for this project featured a server that communicated 
using TCP. The information can be sent to and from a Python client 
application and a Python server application.

The application utilized an SQLite databse to store the data. The 
back-end performed data validation on incoming request.

The server used threads to handle the incoming requests. There 
are some known consistency issues with Python threads when there are 
multiple simultaneous actions being performed on the same tables.
To address this, there was a single 
database worker that handled all writes to the database.

The project was maintained in shared GitHub project. I did help troubleshoot 
the Java GUI and provided some small snippets of code. But the vast majority
of my contribution was to the Python back-end.