---
title: File Conversion
languages:
  - Python
roles:
  - Laboratory Manager
---

#### Summary
These projects consisting of converting or reformatting a data file. 
They saved a lot of time and prevented data errors because analysts no 
longer had to manually make changes to the files. This is a great 
example of a low complexity project that was easy to implement, 
saved time, and prevented errors.

#### Complexity
This was a very low complexity task that I 
was asked to perform many times over the years.

#### Description
These projects are simply rearranging and/or reformatting the data.
Every analytical instrument in the laboratory created its own data file.
Sometimes this data file could be modified using the software provided by
the manufacturers. Sometimes it could not be modified.

In either case, it often required additional processing before it could be read
by data input software. I would simply load in the file (often into a 
[pandas](https://pandas.pydata.org/) dataframe), make the necessary changes, 
and then export the data to a .csv.

In one particular case, the manufacturer wanted to charage an exhorbitant price for 
its data processing software to analyze its data files.
The data files were save with a .kres or .krgr file extension which I had not seen before. 
It turned out that these were just xml files with a different extension, presumably to 
hint the manufacturer's software that the data strucure was different in each of the 2 
kinds of files. In any case, it was then trivial to convert the xml file into a usuable 
csv file. This saved our department money and sped up the data entry process.