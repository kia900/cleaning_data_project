Run analysis overview: code variables in ‘quotes’

run_analysis reads lines from the features.txt to get column labels. ‘lines’

It also reads lines from the y_train.txt for activity labels. ‘row_lines’.

Then it makes a vector (‘vec’) with descriptive names for each activity.

Extract subject codes into lines (‘subject_lines’) from subject_train.txt and add to a vector ‘subject_code’.

to extract mean and std from X_train (‘train_file’), initiate a variable ‘x’ for index of ‘lines’ with the phrase “mean” or “std”. ‘test_ave’ and ‘test_std’ are boolean variables where if True, the x-th column of ‘train_file’ is extracted using the read.fwf command. These columns will be appended to variable ‘data’ with column label ‘names’.

a data frame is then initiated with ‘data’ , row names from ‘vec’ , and column labels ‘names’.

finally ‘vec’ and ‘subject_code’ are added as columns to the data frame from previous step(6).

Steps 1 and 7 are repeated for the Test data set X_test.txt

Train and Test data frames from steps 1-8 are merged back-to-back as ‘df_final’

summary table is made with the ddply command of plyr package. ’summary_table’ and written to a file with the write.table command.
