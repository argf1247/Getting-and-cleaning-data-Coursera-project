Getting-and-cleaning-data-Coursera-project
==========================================

The script does the following:
1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement. 
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names. 
5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject. 

##Process

For both the test and train datasets, produce an interim dataset:
Extract the mean and standard deviation features (listed in CodeBook.md, section 'Extracted Features'). This is the values table.
Get the list of activities.
Put the activity labels (not numbers) into the values table.
Get the list of subjects.
Put the subject IDs into the values table.
Join the test and train interim datasets.
Put each variable on its own row.
Rejoin the entire table, keying on subject/acitivity pairs, applying the mean function to each vector of values in each subject/activity pair. This is the clean dataset.
Write the clean dataset to disk.

================================================================================
Contains the scripts and documents related to the project on the Coursera course
