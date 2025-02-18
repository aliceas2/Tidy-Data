# Codebook for Tidy-Data

## Introduction
One of the most exciting areas in all of data science right now is wearable computing. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. 
The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. 

## Data Sources
* Original Data: ```https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip```
* Description: ```http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones```

## Information
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

## Included Files
* 'README.txt'
* 'Tidy.txt'
* 'Codebook.md'
* 'run_analysis.R'
* 'UCI HAR Dataset'

Note: UCI HAR Dataset is included but the files are not needed if you downloaded as instructed in the README.md file.

## Transformation Details
1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive activity names.
5. Creates independent tidy data set with the average of each variable for each activity and each subject.

## Transformation Implementation
run_analysis.R performs all transformation steps necessary by doing the following.
* Loads all data,
* Loads the labels,
* Extract the mean and standard deviation column names and data,
* Processes both test and train data, 
* Merges the test and train data,
* Creates a 'tidy.txt' file.
