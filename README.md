This code generates a tidy data set of accelerometers from the Samsung Galaxy S smartphone in 5 steps. This is the data:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Here are the steps:

I. GENERATE DATA FRAME TRAIN_DATA: This step makes a data frame of the mean and standard deviation from the Train data. It will also have 2 added columns for the subject and their activities.

II. GENERATE DATA FRAME TEST_DATA: This step is the same as I, but for the Test data.

III. MERGE DATA FRAMES: TRAIN_TEST: This step merges data frame generated from I&II.

IV. GENERATE SUMMARY TABLE: makes a summary table of the merged data frame.

V. SUMMARY TABLE: write summary table.

____________________________________________


Lines 3-9 point to location of the files, read by the function ‘run_analysis’.
To execute, edit lines 3-9, source file at the R console, and type at the command line:

> run_analysis(x)

____________________________________________






