Getting-and-cleaning-data-Coursera-project
==========================================

The script does the following:
- Merges the training and the test sets to create one data set.
- Extracts only the measurements on the mean and standard deviation for each measurement.
- Uses descriptive activity names to name the activities in the data set.
- Appropriately labels the data set with descriptive variable names.
- Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

Uses the following libraries:
- table.data
- reshape2

Uses the following funtions:
- unzip, Extract files from or list a zip archive
- setdiff, Performs set union, intersection, (asymmetric!) difference, equality and membership on two vectors
- grepl,  search for matches to argument pattern within each element of a character vector
- names, Functions to get or set the names of an object
- cbind, Take a sequence of vector, matrix or data frames arguments and combine by columns or rows, respectively
- rbind, Take a sequence of vector, matrix or data frames arguments and combine by columns or rows, respectively
- melt, Convert an object into a molten data frame
- dcast, Use acast or dcast depending on whether you want vector/matrix/array output or data frame output. Data frames can have at most two dimensions.


##Process

For both the test and train datasets produces a new dataset:
- Get the list of activities.
- Put the activity labels (not numbers) into the values table
- Get the list of subjects
- Put the subject IDs into the values table
- Join the test and train datasets
- Put each variable on its own row
- Rejoin the entire table, keying on subject/acitivity pairs, applying the mean function to each vector of values in each subject/activity pair
- Write the clean dataset to disk

================================================================================
Contains the scripts and documents related to the project on the Coursera course
