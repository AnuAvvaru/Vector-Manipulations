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

![](Numeri_Script_files/figure-markdown_strict/pressure-1.png)

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.

Creating a numeric vector
=========================

    patient_id <- c(1001,1002,1003,1004,1005)
    patient_id

    ## [1] 1001 1002 1003 1004 1005

    p_id1 <- c(2001,2002,2003,NA,2005,2006,NA)
    p_id1

    ## [1] 2001 2002 2003   NA 2005 2006   NA

Checking lenght of Objects
==========================

    length(patient_id)

    ## [1] 5

    length(p_id1)

    ## [1] 7

Creating number sequence
========================

    p_in <- c(1:10)
    p_in

    ##  [1]  1  2  3  4  5  6  7  8  9 10

Other way number sequence
=========================

    1:20

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20

    seq(1:50)

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
    ## [24] 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46
    ## [47] 47 48 49 50

Inserting values in Objects by using Seq
========================================

    year1 <- seq(1:50)
    year1

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
    ## [24] 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46
    ## [47] 47 48 49 50

    p_out <- c(1:20)
    p_out

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20

Ojects
======

    ls()

    ## [1] "p_id1"      "p_in"       "p_out"      "patient_id" "year1"

Extracting Index Values
=======================

    p_id1[2]

    ## [1] 2002

    p_in[c(3,4)]

    ## [1] 3 4

    p_out[c(3:30)]

    ##  [1]  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 NA NA NA NA NA
    ## [24] NA NA NA NA NA

Replacing
=========

    p_id1[2] <- p_in[5]
    p_id1

    ## [1] 2001    5 2003   NA 2005 2006   NA

    year1[c(2,10,33,40)] <- patient_id[c(3,4,4,5)]
    year1

    ##  [1]    1 1003    3    4    5    6    7    8    9 1004   11   12   13   14
    ## [15]   15   16   17   18   19   20   21   22   23   24   25   26   27   28
    ## [29]   29   30   31   32 1004   34   35   36   37   38   39 1005   41   42
    ## [43]   43   44   45   46   47   48   49   50

Arithmetic Operations
=====================

Addition
========

    p_in <- c(1:10)

    p_in

    ##  [1]  1  2  3  4  5  6  7  8  9 10

    p_in[c(2,5,10)]+5

    ## [1]  7 10 15

    p_in[1]+2

    ## [1] 3

Adding for particular Index
===========================

    marks=c(22,34,45,56)
    marks

    ## [1] 22 34 45 56

    marks<-marks[2]+10
    marks

    ## [1] 44

Removing Index values
=====================

    p_out

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20

    p_out[-c(2,5)]

    ##  [1]  1  3  4  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20

    last_out <- p_out[length(p_out)-2]
    last_out

    ## [1] 18

    p_out

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20

Subtraction
===========

    days <- 400/30
    days

    ## [1] 13.33333

Assigning vales and Removing some values
========================================

    pay_list <- seq(1:70)
    pay_list

    ##  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
    ## [24] 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46
    ## [47] 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69
    ## [70] 70

    pay_list1 <- pay_list[length(pay_list)-20:length(pay_list)]
    pay_list1

    ##  [1] 50 49 48 47 46 45 44 43 42 41 40 39 38 37 36 35 34 33 32 31 30 29 28
    ## [24] 27 26 25 24 23 22 21 20 19 18 17 16 15 14 13 12 11 10  9  8  7  6  5
    ## [47]  4  3  2  1

Ojects
======

    ls()

    ##  [1] "days"       "last_out"   "marks"      "p_id1"      "p_in"      
    ##  [6] "p_out"      "patient_id" "pay_list"   "pay_list1"  "year1"

Length of Objects
=================

    length(ls())

    ## [1] 10
