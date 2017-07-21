Learning R
========================================================
author: Matthew Cox-Martin
date: 
autosize: true

Learning Objectives
========================================================

- Learn how to better interface with data analysts by learning basic data analysis skills
- Learn how to learn to use **R** and **RStudio**

Analyzing Data
========================================================

- Understanding how data are read in and manipulated can help you be a better researcher
    - How to create databases
    - How new variables are created
    - Knowing which variables are which type
    - Knowing which analyses you can run based on the type of data you have

Data analysis programs
========================================================
Most popular data analysis programs for scholarly articles of 2016

![](H:/Learn R/r-use.png)

http://r4stats.com/articles/popularity/ 


About R
========================================================

R is an open source, object oriented "language and environment for statistical computing and graphics". 

www.r-project.org

R is popular because:
- It's free
- It has a broad support network where users can ask and answer questions
- It is highly adaptable through the use of packages


Parts of the R graphic user interface
========================================================

- Console 
- Editor
- Graphics Device

R user interface
========================================================

<img src="H:/teachr/teachr/LearningR/R-console.png" title="plot of chunk fig2" alt="plot of chunk fig2" width="100%" />


R studio
========================================================

The basic R GUI is not optimized for users

**RStudio** is a separate integrated development environment that enhances the usability of R in several ways

Basic enhancements from R studio include:

  - Easier navigation of multiple scripts, plots, packages, and global environment
  - Code completion
  - Color coding of code
  - Easier debugging


R studio (cont)
========================================================

The most useful elements of R studio include:

- Projects (grouping all related R files and workspaces together)

- Version control (through Git or other service)

- Shiny app (interactive controls and figures)

- Markdown (R Markdown, R Presentations, R HTML, etc.)


Install R
========================================================

- Go to www.r-project.org and click "download R"
- Select a server from which to download **R** (try https://cloud.r-project.org/)
- Select the link for the operating system you are using
    - If you're using Windows click "install R for the first time" and the click the link that begins "Download..."
    - For Mac users, click on the first link in the left column under "Files:"


Install RStudio
========================================================

- Go to https://www.rstudio.com/
- Click "RStudio"
- Click "Desktop"
- Click "DOWLOAD RSTUDIO DESKTOP"
- Scroll to the bottom and and select the link that has your operating system
- NOTE: RStudio changes their layout so these steps might not always be the same


About R
========================================================

**R** is similar to **SAS** and other code-based stat programs

One big difference
- **R** uses object-oriented programming
    - This allows for indexing to access elements of objects (including vectors, matrices, lists, and dataframes)
    - I can save an analysis as an object and use the indices to pull values (coefficients and standard errors) to make a table or conduct further analyses


Object orient programming
========================================================

- Objects are a way of organizing and accessing data
    - Data here means anything you can input or output from **R**

Imagine a filing cabinet where you store the relevant papers in your life.  If you need your tax returns from last year, you find the filling cabinet, open the correct drawer, find the properly labeled folder, and pull out the file.  This is, in princple, how object orient programming works.  Objects can be any type of data that **R** can handle including graphs, output, tables, numbers, characters, etc.

- Go to the first example on the Tutorial worksheet to learn about objects in **R**


Data in R
========================================================

- For any stats software there are basic formatting requirements for data 
- http://ropensci.github.io/reproducibility-guide/sections/dataSharing/
    - Each variable you measure should be in one column
    - Each different observation of that variable should be in a different row
    - Each table/file should be it's own dataset
    - If you have multiple tables, they should include a column in the table that allows them to be linked


Data in R (cont.)
========================================================
Messy Data

|       | pregnant| not_pregnant|
|:------|--------:|------------:|
|Male   |        0|            5|
|Female |        1|            4|

Tidy Data 

|pregnant |sex    | freq|
|:--------|:------|----:|
|no       |female |    4|
|no       |male   |    5|
|yes      |female |    1|
|yes      |male   |    0|


Packages
========================================================

Packages are programs that other users have created which can be added to the base R system in order to increase functionality (similar to MACROS in **SAS**)

Packages are like apps for your phone

- First download and install a package 


```r
install.packages("ggplot2")
```

- Then load the package


```r
library(ggplot2)
```

Packages need to be loaded every time you restart R and it is usually good practice to reinstall them so that they update


Packages (cont)
========================================================

Packages are downloaded from the Comprehensive R Archive Network (CRAN)

There are currently (as of 5/17/16) 11110 packages available from from CRAN (7000 have been added in the last 6 years)

https://cloud.r-project.org


Resources for learning and getting help with R
========================================================

I have a large compendium of PDFs and links to helpful R resources that I am happy to share

Most problems can be solved through Google

Can use the help() function to direct you to the corresponding help page for the respective function
- All **R** packages and base functions have a manual (referenced online) with examples on how to use them

There are several places on the internet where you can learn **R** through a structured course for free or very little money using **Coursera**, **Udemy**, or **DataCamp** (even YouTube has many helpful videos).  


