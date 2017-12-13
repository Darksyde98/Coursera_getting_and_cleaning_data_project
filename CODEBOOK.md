CodeBook for the tidy dataset
-----------------------------

### Data source

This dataset is derived from the "Human Activity Recognition Using
Smartphones Data Set" which was originally made available here:
<http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones>

### Feature Selection

Please refer to the README and features.txt files in the original for
more detail regarding the dataset beyond what is given here.

The features selected for this database come from the accelerometer and
gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain
signals (prefix 't' to denote time) were captured at a constant rate of
50 Hz. Subsequently, the body linear acceleration and angular velocity
were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and
tBodyGyroJerk-XYZ).

Finally a Fast Fourier Transform (FFT) was applied to some of these
signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ,
fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to
indicate frequency domain signals). The logic behind this selection of
features is that the assignment explicitly states "Extract only the
measurements on the mean and standard deviation for each measurement."

In short, for this derived dataset, these signals were used to estimate
variables of the feature vector for each pattern:

'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions. 

-       tBodyAcc-XYZ 
-       tGravityAcc-XYZ 
-       tBodyAccJerk-XYZ 
-       tBodyGyro-XYZ 
-       tBodyGyroJerk-XYZ 
-       tBodyAccMag 
-       tGravityAccMag 
-       tBodyAccJerkMag 
-       tBodyGyroMag 
-       tBodyGyroJerkMag 
-       fBodyAcc-XYZ 
-       fBodyAccJerk-XYZ 
-       fBodyGyro-XYZ 
-       fBodyAccMag 
-       fBodyAccJerkMag 
-       fBodyGyroMag 
-       fBodyGyroJerkMag

From these signals the following variables were kept: 

-       mean(): Mean value 
-       std(): Standard deviation

Additional vectors obtained by averaging the signals in a signal window
sample. 

-       gravityMean 
-       tBodyAccMean 
-       tBodyAccJerkMean 
-       tBodyGyroMean
-       tBodyGyroJerkMean

**Note:** features are normalized and bounded within \[-1,1\].

The resulting variable names are of the following form: tbodyaccmeanx,
which means the mean value of tBodyAcc-XYZ.
