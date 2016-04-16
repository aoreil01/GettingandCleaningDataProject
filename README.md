# Getting and Cleaning Data Project

    This repo explains how all of the scripts work and how they are connected.

    You should create one R script called run_analysis.R that does the following.

    1. Merges the training and the test sets to create one data set.
    2. Extracts only the measurements on the mean and standard deviation for each measurement.
    3. Uses descriptive activity names to name the activities in the data set
    4. Appropriately labels the data set with descriptive variable names.
    5. From the data set in step 4, creates a second, independent tidy data set with the average 
    of each variable for each activity and each subject.
    
testTrain
        All 6 datasets (test.labels, test.subjects, test.data, train.labels, train.subjects & train.data)
        combined into a single data frame.

features

        The features.txt as a table

features.mean.std

        The features table with all columns except those with "mean" or "std" removed.

data.mean.std

        The data from testTrain that includes only the columns in the features.mean.std table.

labels

        The activity_labels.txt file as a table

good.colnames

        A list of the column names from the features.mean.std table, in lower case with all 
        alphanumeric chracters removed.

aggr.data

        a data frame that includes only the mean values for each subject for each column.

