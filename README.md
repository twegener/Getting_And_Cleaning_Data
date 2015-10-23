---
title: "README.md"
output: html_document
---

Coursera - Getting and Cleaning Data - Project
==============================================

This repository hosts all R code and the documentation files for Coursera's Data Science track course "Getting and Cleaning data".

The dataset being used is: [Human Activity Recognition Using Smartphones](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)


Project relevant data files are: [Human Activity Using Smartphones - Datafiles](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)


## Files

The code takes for granted all the data is present in the set WorkDir folder and without any names altered. If only ZIP file is available it will be unzipped.

`CodeBook.md` describes the variables, the data, and any transformations or work that were performed to clean up the data.

`run_analysis.R` contains all the code to perform the following 5 steps:

1. Merges the training and the test sets to create one data set.

2. Extracts only the measurements on the mean and standard deviation for each measurement.

3. Uses descriptive activity names to name the activities in the data set.

4. Appropriately labels the data set with descriptive variable names.

5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

They can be launched in RStudio by importing the file.

The output of the 5th step is called `tidy.txt`, and uploaded in the course project's form.

