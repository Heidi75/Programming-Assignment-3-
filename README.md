# Programming-Assignment-3-
This is easy to understand instructions for people who don't like to read.   For Programming assignment 3 in R Programming by Johns Hopkins University Programming for the John
PROGRAMMING ASSIGNMENT 3
R Programming


Directions:
  Plot the 30-day mortality rate for heart attack
Print Hospital_Revised_Flatfiles.pdf at least the pages with Number 19 “Outcome of Care Measure.cvs” and Number 11 “Hospital_Data.cvs”
Take note that the numbers of the variables for each table indicate column indices in each table ie.  “Hospital Name” is column 2 in the Number 19 “Outcome of Care Measure.cvs” 
outcome <- read.csv("outcome-of-care-measures.csv", colClasses = "character")
colClasses in read.cvs manually sets the data types for each column
head(outcome) 
head(data.frame) you get the first few records from all the columns displayed.
ncol(outcome)
ncol() function returns the number of columns of a matrix. 
nrow() function returns the number of rows of a matrix.
names(outcome)
Displays the names of each column
outcome[, 11] <- as.numeric(outcome[, 11])
as.numeric - change the characteristics of variables in a dataframe
as.factor- change the characteristics of variables in a dataframe
So we dataframe we are working with “outcome” we are coercing the dataframe outcome to make a new dataframe as numeric.   We converted the characteristics of the variables of “character” to numeric
hist(outcome[, 11]) - Histogram can be created using the hist() function in R programming language. This function takes in a vector of values for which the histogram is plotted.
