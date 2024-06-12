---
title: Discard List Report
roles:
  - Laboratory Data Manager
  - Laboratory Manager
languages:
  - Python
tools:
  - Git
---

#### Summary
This project utilized Python to create a sample discard list.
This list was generated based on the time since samples
were validated and the contents that were found in the sample.
Any unknonwn chemicals will open a website with the chemical information
and the user can enter the discard status for that chemical. This will 
be remembered for future executions.

#### Description
This is a relatively simple command line program. The program 
reads in a csv file with the sample data. It analyzes the data 
to determine which samples are ready to be discarded. This determination
is based on how long it has been since the samples were validated.

From there, the contents of the sample are analyzed. Based on the 
chemicals that were identified in the sample, different sample
discard proceedures must be followed.

The program used an external file to store information about
which chemicals require which displosal type. However, there 
are many different names for chemicals and many different chemicals. 
Rather than attempt to list every possible chemical name, I simply started with 
a list of common checmicals and their discard status.

If the program encounters a chemical 
it does not recognize, it opens a website with the chemical information.
The user can then indicate what the discard status for that chemical is based on
the website or other information sources. The program stores the 
new chemical discard status in the external file so that it
will be available in future executions.