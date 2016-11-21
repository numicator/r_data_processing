Title: Data Processing in R
Author: Marcin Adamski
Affiliation: CBBU, RSB ANU
Date: 18-11-2016

# *** Data Processing in R ***

### Time: Two 6 hour sessions
> The first session is for beginners, the second for more advanced users.

## Learning objectives:
1. Data types in R, and type conversions.
2. Loading and saving tab and coma delimited files.
3. Detecting and handling errors an missing values in the data.
4. Data sub-setting and filtering.
5. Adding new columns with calculated values.
6. Writing functions.
7. Traversing data with the apply functions.
8. Data reshaping with _tidyr_.
9. Data processing with _dplyr_.

---
*** First 6-hours session: ***
---

## Brief introduction to R and RStudio.
 - RStudio IDE (Integrated Development Environment).
 - Help in R and RStudio.
 - Concept of an RStudio project.

## Data types in R, and type conversions.
 - Atomic vectors.
 - Type conversions and coercions.
 - Working with date and date-time formats.

## Working with files:
 - How to organize your directory structure.
 - Downloading files form the web.
 - Reading data files.
 - Writing dta files.

```
Exercise 1: Processing of a 'dirty' dataset - finding and correcting errors. 
We will be working on a dataset containing some errant data. We will learn 
ways of finding and correcting or deleting incorrect records. We will 
find-and-replace values, create new columns and delete existing ones. Then we 
will write corrected dataset on the disk.
```

## Data reshaping with _tidyr_ package:
 - The 'normal' data format for statistical analyses: column represent variables, rows represent observation.
 - The 'wide', or spreadsheet format.
 - Conversion from wide to normal with _gather()_, _separate()_ and _spread()_ functions

```
Exercise 2: Converting a spreadsheet-like data file into a 'normal' format 
for statistical analyses.
```

## Data processing with _dplyr_ package:
  - _dplyr_ and the data processing workflow: split - apply - combine.
  - Selecting columns and filtering rows.
  - Creating new columns.
  - Concept of a pipe and the pipe operator.
  - Grouping observations and summarizing.
  - Joining data: inner, left, right, semi, anti joins.
  - Accessing remote SQL databases.

```
Exercise 3: We will use a data set containing three tables (files). 
We will learn how to join the data files together using dplyr. How to filter 
observations, choose columns, calculate new columns, and change scope of the 
analysis (grouping observations by factors).
```

```
Exercise 4: We will learn how to connect to an external, remote SQL database.
We will use the Ensembl genome browser database and an example.
```

## Other functions for joining datasets:
 - _dplyr_ functions: _bind_cols()_, _bind_rows()_, _union()_, _intersection()_, and _set_diff()_
 - base functions: _cbind()_, _rbind()_, _merge()_, _union()_, _intersect()_, _setdiff()_

---
*** Second 6-hours session: ***
---

# Writing functions in R:
 - What is a function and when is it useful?
 - Function elements - name, definition, arguments, body, return value.
 - Special functions: Infix and replacement

```
Exercise 5: We will write a function calculating area under a curve given 
as a set of (x-y) points. The area (the integral) will be numerically 
calculated using the trapezoid rule. Then we will test our new function on 
a test dataset (which we first create).
```

# Applying functions to the data - the 'apply' family of functions:
 - short presentation of the family members with special focus on _apply()_, _lapply()_, and _sapply()_

```
Exercise 6: We will learn use of apply functions by processing two datasets: 
We will traverse the data column-by-column and row-by-row. We will write our 
own functions to be applied for each row and column.
We will learn that we do not always need to explicitly name a function 
- instead we can use anonymous function for small tasks. We will also see 
some tricks and nuisances associated with the apply functions.
```

# Processing multiple files:
 - Listing directory, getting list of files.
 - Processing files one-by-one using the _for_ loop.

```
Exercise 7: We will download a ZIP archive containing numerous files with 
gene expression data. We will learn how to unzip it directly from R, get 
their names and process them interactively: We will collect a specific column 
from each of the files and create a new file with combined data - a data 
expression matrix file.
```
---
*** End of the workshop***
---

