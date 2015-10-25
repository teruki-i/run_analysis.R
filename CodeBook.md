##Explanation of original data
This code uses data collected from accelerometers from the Samsung Galaxy S smartphone.

The original study collected data from 30 subjects walking, walking upstairs, walking downstairs, sitting, standing, and laying and took various measures of their motions.

##Explanation of variables for column 1 and 2

subject: number used to identify subject (1~30)
activity: indicates activiy measured (walking, walking upstairs, walking downstairs, sitting, standing, laying)

##Explanation of variables for columns 3-68
NOTE: columns 3-68 are the AVERAGES of the variables explained below and not the actual measures from the original study

Measures for the motion were taken in all three dimensions.
The "X," "Y," and "Z" appended to variable names indicate which direction the measure was taken.

Variables with "Acc" in the name come from the accelerometer while those with "Gyro" come from the gyrocope

Variables with a "t" prefix indicate time domain signals. The original variables were capurted at a constant rate of 50Hz

Body linear acceleration and angular velocity were derived in time to obtain Jerk signals.
Variables with "BodyAccJerk" in the name are for the body linear acceleration while those with "GravityAcc" in the name are for the angular velocity

The magnitude for the three-dimensional signals were also calculated using the Eucledian norm.
Variables with the "t" prefix and "Mag" in the name are for these magnitudes.

A Fast Fourier Transform (FFT) was applied to some of these signals.
Variables with a "f" prefix in the name are for these transforms.
"f" indicates frequency domain signals.

Finally, only the means and standard deviations for all these variables are included in this data set.
Variables with "mean()" in the name are for the means.
Variables with "std()" in the name are for the standard deviations.

##Regarding exluded variables

As this assignment specifically asked only for variables that measured mean and standard deviation, the final tidy data sets exclude the variables multiple variables included in the original data set. For example, this does not include entropy() for signal entropy or meanFreq() for weighted average of the frequency components to obtain mean frequency.

Furthermore, for sake of simplicity, the variables that had the following components in the names were also excluded: gravityMean, tBodyAccMean, tBodyAccJerkMean, tBodyGyroMean, and tBodyGyroJerkMean.These variables were created by averaging the signals in a signal window sample

To see a full list of variables from the original study and further explanation on them, please refer to feature.txt and features_info.txt from original data folders.
