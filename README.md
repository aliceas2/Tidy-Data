# Tidy-Data
## Project for Getting and Cleaning Data Course

The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set.

## Deliverables
You should create one R script called run_analysis.R that does the following.

1) Merges the training and the test sets to create one data set.
2) Extracts only the measurements on the mean and standard deviation for each measurement.
3) Uses descriptive activity names to name the activities in the data set
4) Appropriately labels the data set with descriptive variable names.
5) From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## Set Up
There is minimal setup required. To set up, do the follwoing.

1) Download the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.
2) Extract the files to your desired location.
3) Set your working directory to the parent directory of the downloaded folder ```UCI HAR Dataset```
4) Place ```run_analysis.R``` in the parent directory of the downloaded folder ```UCI HAR Dataset```
5) Run ```source("run_analysis.R")``` 
6) Running the script will create a tidy data file called ```tidy.txt``` in your working directory.
