The dataset includes the following files:
=========================================

- 'README.md'

- 'run_analysis.R': An R script that performs the analysis.
 
- 'tidydata.txt': Tidy data set

- 'CodeBook.md': A file describes the variables, the data, and any transformations/work that I performed to clean up the data.


run_analysis.R
==============
Download the data for the project using the link: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
Unzip the file.
Moved the files into a folder 'UCI HAR Dataset' in the working directory.

Get the list of files into the variable 'files'

Step 1 
------
Merged the training and the test sets to create one data set.

Read data from the files into the variables: dataActivityTest,  dataActivityTrain, dataSubjectTrain,  dataSubjectTest, dataFeaturesTest,  dataFeaturesTrain  
Concatanate the data tables by rows: dataActivity, dataSubject, dataFeatures
Set names to variables.
Merged columns to get the data frame: 'Data'

Step 2
------
Extracted only the measurements on the mean and standard deviation for each measurement.

Created a new data frame with extracted data: 'Q2subsetData'

Step 3
------
Used descriptive activity names to name the activities in the data set 'Q2subsetData'.

Step 4
------
Appropriately labeled the data set 'Q2subsetData' with descriptive variable names.

Step 5
------
From the data set in step 4, created an independent tidy data set 'Q5Data' with the average of each variable for each activity and each subject.
Saved that data frame in the file 'tidydata.txt'.
