# q2-chemistry 

---

### Introduction

--- 

This package contains the source code for a plug-in for Qiime2 to be able to interact and be used with molecular 
dynamics simulation software such as Amber, packmol, tleap, and etc. It also will contain various tools 
for the analyses of these simulations such as looking at the Total Enery Levels of a reaction and examining
a structures density overmicroscopic time increments. Currently the main tool is a parser which can transform 
a text based .out file produced by amber simulations, and parse it into a pandas dataframe to be used however 
the researcher might need. This is intended purely to give a more useful description and format for the data 
to be analyzed computationally. Without this tool it is difficult to do heavy analyses on these files as they 
are only human readable and not useable easily as values are not in a table format.

---

### Installation 

---

This package is a WIP but eventually will be deployed either alongside the base qiime2 framework or as a 
standard Qiime2 plug-in which can be incorporated through conda or pip/using git. Currently the best way to
utilize this package is by importing the chemparser.py file into a jupyter or ipython environment so that
its function's and pipelines can be utilized right away. In the future this will change to a full form qiime2
plugin which can be used like any other qiime2 plugin; reference qiime2.org to learn more about this software tool.

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
If you utilize q2-chemistry for any published research please include the following citation:
