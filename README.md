# q2-chemistry 

---

### Introduction

--- 

This repo contains source code for a data parser for a typical .out file created from amber molecular dynamic simulations. This allows the user to examine their data inside of a datastructure which gives them more power to do an analysis.

---

### Installation 

---

Simply clone this repository and follow along with the jupyter notebook to see how this package works

---

### Users

---

Initially the first tool in most situations will be to take your amber/pmemd simulation's .out file and parse it into a dataframe using the parse_pl() function. This can be done in a few different ways:

->start up ipython/jupyter.<-

->type `import chemparser`.   NOTE: Your working directory for this step must be the same directory which contains the chemparser.py file.<-

->use the parse_pl() function to create a dataframe from a .out file. For example: `parse_pl("/chemsims/equil.out")`, the inside of the function is a string with the .out file's path from the current working directory<-

This pipeline should return the dataframe, thus it can be assigned to a variable to hold the dataframe:

->`chemdataframe = parse_pl(/chemsims/equil.out`<-

Now the dataframe contained in chemdataframe can be used to perform various analyses and calculations.

---

### Developers

---

Please look at the linked developer documentation and Qiime developer documentation to learn more about how
to contribute to the project or build your own research related tools.

---

### Citing q2-chemistry 

---
If you utilize this script for any published research please include the following citation:
