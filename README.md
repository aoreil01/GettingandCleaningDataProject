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

The script follows the steps outlined in the assignment

    1. Merges the training and the test sets to create one data set.

All six data sets are merged into a sing data frame called testTrain

    2. Extracts only the measurements on the mean and standard deviation for each measurement.
    
The features.txt file is read into a table called features.
the features tables is filtered for only data that contains 'mean' or 'std' and placed into a table
called features.mean.std, which is then used to filter out columns in the testTrain data frame, and produces the data.mean.std data frame.
    
    3. Uses descriptive activity names to name the activities in the data set
    
The activity_labels.txt file is read into a table called labels which are used to replace the names of the activites in data.mean.std
    
    4. Appropriately labels the data set with descriptive variable names.

The column names are extracted out of the data.mean.std and cleaned so that they are lower case and non-alphanumeric
characters are removed. this finished the non-aggregated data frame.
    
    5. From the data set in step 4, creates a second, independent tidy data set with the average 
    of each variable for each activity and each subject.
    
A data frame is created called aggr.data with the data from data.mean.std but aggregated as the mean of the values for each subject. 
