R Markdown
----------

This is an R Markdown document. Markdown is a simple formatting syntax
for authoring HTML, PDF, and MS Word documents. For more details on
using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that
includes both content as well as the output of any embedded R code
chunks within the document. You can embed an R code chunk like this:

    summary(cars)

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

Including Plots
---------------

You can also embed plots, for example:

![](Character_Manipulation_files/figure-markdown_strict/pressure-1.png)

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.

Assigning character Object in Single quotes
===========================================

    Emp_Name <- c('Anu','Sai','Rasool','Srinath','Ankitha','Shasha')
    Emp_Name

    ## [1] "Anu"     "Sai"     "Rasool"  "Srinath" "Ankitha" "Shasha"

Assigning character Object in Double quotes
===========================================

    Flower <- c("Rose","Lily","Sunflower","Daisy","Hibiscus")
    Flower

    ## [1] "Rose"      "Lily"      "Sunflower" "Daisy"     "Hibiscus"

Creating a sentence in Object
=============================

    Quote <- "Keep Smiling"
    Quote

    ## [1] "Keep Smiling"

    Sentence <- "I'm staying at BTM"
    Sentence

    ## [1] "I'm staying at BTM"

Logical Operator
================

    Yes <- T
    Yes

    ## [1] TRUE

    No <- F
    No

    ## [1] FALSE

What Objects are their Environment
==================================

    ls()

    ## [1] "Emp_Name" "Flower"   "No"       "Quote"    "Sentence" "Yes"

Finding Objects are in which Data type
======================================

    class(Emp_Name)

    ## [1] "character"

    class(Flower)

    ## [1] "character"

    class(No)

    ## [1] "logical"

    class(Quote)

    ## [1] "character"

    class(Sentence)

    ## [1] "character"

    class(Yes)

    ## [1] "logical"

Apha\_Numeric
=============

    Emp_ID <- c('Anu1001','Sai1002','Rasool1003')
    Emp_ID

    ## [1] "Anu1001"    "Sai1002"    "Rasool1003"

Replacing one object values to other object
===========================================

    Emp_ID[2] <- Flower[c(3)]
    Emp_ID

    ## [1] "Anu1001"    "Sunflower"  "Rasool1003"

Caluculating lenght of objects
==============================

    length(Emp_ID)

    ## [1] 3

    length(Emp_Name)

    ## [1] 6

    length(Flower)

    ## [1] 5

    length(No)

    ## [1] 1

    length(Yes)

    ## [1] 1

    length(Quote)

    ## [1] 1

    length(Sentence)

    ## [1] 1

Removing Last element in one Object
===================================

    Emp_Name[-c(2,6)]

    ## [1] "Anu"     "Rasool"  "Srinath" "Ankitha"
