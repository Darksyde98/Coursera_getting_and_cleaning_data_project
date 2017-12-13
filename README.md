# Getting and Cleaning Data: Course Project

## Introduction

This repository contains the course project for the Coursera course "Getting and Cleaning data".

## About the raw data

The 561 features of the dataset are unlabeled and can be found in x_test.txt, while the labels are found in the y_test.txt file. Finally the test subjects are found in the subject_test.txt file.

This is true for both the training and test set.

## About the script and the tidy dataset

The script is called run_analysis.R and will merge the test and training sets together. 

### Prerequisites for this script:

- the UCI HAR Dataset must be extracted and..
- the UCI HAR Dataset must be availble in a directory called "UCI HAR Dataset"

The script merges the data and adds labels before removing any values not related to the mean and standard deviation of the data.

In the end the script will create a tidy data set containing the means of all the columns per test subject and per activity. This tidy dataset is found in the delimited file tidy.txt.

### About the Code Book

The CodeBook.md file explains the transformations performed and the resulting data and variables.
