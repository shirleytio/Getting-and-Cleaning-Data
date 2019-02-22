###Summary

This project allows creating a "clean" data set from the 'UCI HAR Dataset' available at:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

It merges different subsets of this data into one single transformed data set --- named "tidydata" --- in order to allow performing data analysis tasks more easily. 


###Execution of script

The script executes the following steps:

1. Load the individual data files of the training and test sets and merge them into one data table.

2. Filter the data table to select only mean and standard deviation columns.

3. Load labels and levels of the activity column and convert the variable into a factor variable.

4. Assign cleaned feature strings as column names for the feature measurements.

5. Merge test and training subsets into one final cleaned data set.

6. Create another derived data set with average values of each measurement variable for each activity and each subject.


###Other requirements 

The script uses the following R packages which need to be available/installed:

1. data.table
2. dplyr