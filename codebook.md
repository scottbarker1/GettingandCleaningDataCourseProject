Codebook for run_analysis.R

The "run_analysis.R" script performs the following steps:

Assumption: 
The data files have been pre-pulled already from the the link "https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip" link and put it in the working directory. 

Transformation of data:

# Install the "plyr" package to obtain the "plyr" functions
###############################################################################

# Step 1
# Merge the training and test sets to create one data set
###############################################################################

# Step 2
# Extract only the measurements on the mean and standard deviation for each measurement
###############################################################################

# Step 3
# Use descriptive activity names to name the activities in the data set
###############################################################################

# Step 4
# Appropriately label the dataset with descriptive variable names
###############################################################################

# Step 5
# Create a second, independent tidy data set with the average of each variable(mean & standard deviation)
# for each activity and each subject.  The data is written from a dataset into CSV file.


=================

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.


Data Columns:
Subject  - The person for which the activity is measuring
        class = integer
Activity   - Physical Activity being tracked
        class = Factor w/6 levels
Values: 1 WALKING
        2 WALKING_UPSTAIRS
        3 WALKING_DOWNSTAIRS
        4 SITTING
        5 STANDING
        6 LAYING

The set of variables that were estimated from these signals are: 

mean(): Mean value
std(): Standard deviation
Class for all variables is number

1 tBodyAcc-mean()-X
2 tBodyAcc-mean()-Y
3 tBodyAcc-mean()-Z
4 tBodyAcc-std()-X
5 tBodyAcc-std()-Y
6 tBodyAcc-std()-Z

7 tGravityAcc-mean()-X
8 tGravityAcc-mean()-Y
9 tGravityAcc-mean()-Z
10 tGravityAcc-std()-X
11 tGravityAcc-std()-Y
12 tGravityAcc-std()-Z

13 tBodyAccJerk-mean()-X
14 tBodyAccJerk-mean()-Y
15 tBodyAccJerk-mean()-Z
16 tBodyAccJerk-std()-X
17 tBodyAccJerk-std()-Y
18 tBodyAccJerk-std()-Z

19 tBodyGyro-mean()-X
20 tBodyGyro-mean()-Y
21 tBodyGyro-mean()-Z
22 tBodyGyro-std()-X
23 tBodyGyro-std()-Y
24 tBodyGyro-std()-Z

25 tBodyGyroJerk-mean()-X
26 tBodyGyroJerk-mean()-Y
27 tBodyGyroJerk-mean()-Z
28 tBodyGyroJerk-std()-X
29 tBodyGyroJerk-std()-Y
30 tBodyGyroJerk-std()-Z


31 tBodyAccMag-mean()
32 tBodyAccMag-std()

33 GravityAccMag-mean()
34 tGravityAccMag-std()

35 tBodyAccJerkMag-mean()
36 tBodyAccJerkMag-std()

37 tBodyGyroMag-mean()
38 tBodyGyroMag-std()

39 tBodyGyroJerkMag-mean()
40 tBodyGyroJerkMag-std()

41 fBodyAcc-mean()-X
42 fBodyAcc-mean()-Y
43 fBodyAcc-mean()-Z
44 fBodyAcc-std()-X
45 fBodyAcc-std()-Y
46 fBodyAcc-std()-Z

47 fBodyAccJerk-mean()-X      
48 fBodyAccJerk-mean()-Y      
49 fBodyAccJerk-mean()-Z      
50 fBodyAccJerk-std()-X       
51 fBodyAccJerk-std()-Y        
52 fBodyAccJerk-std()-Z      

53 fBodyGyro-mean()-X          
54 fBodyGyro-mean()-Y          
55 fBodyGyro-mean()-Z         
56 fBodyGyro-std()-X           
57 fBodyGyro-std()-Y           
58 fBodyGyro-std()-Z  

59 fBodyAccMag-mean()          
60 fBodyAccMag-std() 

61 fBodyBodyAccJerkMag-mean()
62 fBodyBodyAccJerkMag-std()

63 fBodyBodyGyroMag-mean()     
64 fBodyBodyGyroMag-std()     
65 fBodyBodyGyroJerkMag-mean()
66 fBodyBodyGyroJerkMag-std() 
