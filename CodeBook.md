---
title: "CodeBook.md"
author: "TW"
date: "23. Oktober 2015"
output: html_document
---
# Introduction

The script `run_analysis.R`performs the 5 steps described in the course project's definition.

1. Merges the training and the test sets to create one data set.

2. Extracts only the measurements on the mean and standard deviation for each measurement.

3. Uses descriptive activity names to name the activities in the data set.

4. Appropriately labels the data set with descriptive variable names.

5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

# Variables

## Directory & File Names
- source_file contains name of comprehensive ZIP file.
- wd contains Work Directory.

## Labels & Features Data
- activityLabels contains activity data from "UCI HAR Dataset/activity_labels.txt"
- features contains features data from "UCI HAR Dataset/features.txt"


## Extract the data on mean and standard deviation
- featuresWanted contains mean and standard deviation selection criteria.


## Load & combine (column bind) training & test datasets separately
- train firstly contains data from file "UCI HAR Dataset/train/X_train.txt" for featuresWanted selection criteria; then it becomes combined with trainActivities and trainSubjects as per below.

- trainActivities contains data from file "UCI HAR Dataset/train/Y_train.txt".

- trainSubjects contains data from "UCI HAR Dataset/train/subject_train.txt".

- test firstly contains data from file "UCI HAR Dataset/test/X_test.txt" for featuresWanted selection criteria; then it becomes combined with testActivities and testSubjects as per below.

- testActivities contains data from file "UCI HAR Dataset/test/Y_test.txt".

- testSubjects contains data from "UCI HAR Dataset/test/subject_test.txt".

## merge train & test datasets (row bind) and add labels
allData contains combined training and test data with corresponding column labels as well as melted and mean data.
