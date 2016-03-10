#Codebook

#Raw Data Collection

###Data Set Information
The experiments were carried out with a group of 30 volunteers within an age bracket of 19-48 years. They performed a protocol of activities composed of six basic activities: three static postures (standing, sitting, lying) and three dynamic activities (walking, walking downstairs and walking upstairs). The experiment also included postural transitions that occurred between the static postures. These are: stand-to-sit, sit-to-stand, sit-to-lie, lie-to-sit, stand-to-lie, and lie-to-stand. All the participants were wearing a smartphone (Samsung Galaxy S II) on the waist during the experiment execution. We captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz using the embedded accelerometer and gyroscope of the device. The experiments were video-recorded to label the data manually. The obtained dataset was randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of 561 features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

###Attribute Information

The dataset is then divided in two parts and they can be used separately. 

Inertial sensor data:
* Raw triaxial signals from the accelerometer and gyroscope of all the trials with with participants. 
* The labels of all the performed activities. 

Records of activity windows. Each one composed of: 
* A 561-feature vector with time and frequency domain variables. 
* Its associated activity label. 
* An identifier of the subject who carried out the experiment. 

###Raw Data Collection
Raw data are obtained from UCI Machine Learning repository:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

#ID Fields

subject - Participant ID
activity - Label of activity performed when measurements were recorded

#Feature Fields

*tBodyAcc-mean()-X 
*tBodyAcc-mean()-Y 
*tBodyAcc-mean()-Z 
*tBodyAcc-std()-X 
*tBodyAcc-std()-Y 
*tBodyAcc-std()-Z 
*tGravityAcc-mean()-X 
*tGravityAcc-mean()-Y 
*tGravityAcc-mean()-Z 
*tGravityAcc-std()-X 
*tGravityAcc-std()-Y 
*tGravityAcc-std()-Z 
*tBodyAccJerk-mean()-X 
*tBodyAccJerk-mean()-Y 
*tBodyAccJerk-mean()-Z 
*tBodyAccJerk-std()-X 
*tBodyAccJerk-std()-Y 
*tBodyAccJerk-std()-Z 
*tBodyGyro-mean()-X 
*tBodyGyro-mean()-Y 
*tBodyGyro-mean()-Z 
*tBodyGyro-std()-X 
*tBodyGyro-std()-Y 
*tBodyGyro-std()-Z 
*tBodyGyroJerk-mean()-X 
*tBodyGyroJerk-mean()-Y 
*tBodyGyroJerk-mean()-Z 
*tBodyGyroJerk-std()-X 
*tBodyGyroJerk-std()-Y 
*tBodyGyroJerk-std()-Z 
*tBodyAccMag-mean() 
*tBodyAccMag-std() 
*tGravityAccMag-mean() 
*tGravityAccMag-std() 
*tBodyAccJerkMag-mean() 
*tBodyAccJerkMag-std() 
*tBodyGyroMag-mean() 
*tBodyGyroMag-std() 
*tBodyGyroJerkMag-mean() 
*tBodyGyroJerkMag-std() 
*fBodyAcc-mean()-X 
*fBodyAcc-mean()-Y 
*fBodyAcc-mean()-Z 
*fBodyAcc-std()-X 
*fBodyAcc-std()-Y 
*fBodyAcc-std()-Z 
*fBodyAccJerk-mean()-X 
*fBodyAccJerk-mean()-Y 
*fBodyAccJerk-mean()-Z 
*fBodyAccJerk-std()-X
*fBodyAccJerk-std()-Y 
*fBodyAccJerk-std()-Z 
*fBodyGyro-mean()-X 
*fBodyGyro-mean()-Y 
*fBodyGyro-mean()-Z
*fBodyGyro-std()-X 
*fBodyGyro-std()-Y 
*fBodyGyro-std()-Z 
*fBodyAccMag-mean() 
*fBodyAccMag-std() 
*fBodyBodyAccJerkMag-mean() 
*fBodyBodyAccJerkMag-std() 
*fBodyBodyGyroMag-mean() 
*fBodyBodyGyroMag-std() 
*fBodyBodyGyroJerkMag-mean() 
*fBodyBodyGyroJerkMag-std() 

#Activity Labels

*WALKING (value 1)
*WALKING_UPSTAIRS (value 2)
*WALKING_DOWNSTAIRS (value 3)
*SITTING (value 4)
*STANDING (value 5)
*LAYING (value 6)

#Vectors

##Extracted Features Vector

c(1, 2, 3, 4, 5, 6, 41, 42, 43, 44, 45, 46, 81, 82, 83, 84, 85, 86, 121, 122, 123, 124, 125, 126, 161, 162, 163, 164, 165, 166, 201, 202, 214, 215, 227, 228, 240, 241, 253, 254, 266, 267, 268, 269, 270, 271, 345, 346, 347, 348, 349, 350, 424, 425, 426, 427, 428, 429, 503, 504, 516, 517, 529, 530, 542, 543)

##Extracted Feature Names Vector

c("tBodyAcc-mean()-X", "tBodyAcc-mean()-Y", "tBodyAcc-mean()-Z", "tBodyAcc-std()-X", "tBodyAcc-std()-Y", "tBodyAcc-std()-Z", "tGravityAcc-mean()-X", "tGravityAcc-mean()-Y", "tGravityAcc-mean()-Z", "tGravityAcc-std()-X", "tGravityAcc-std()-Y", "tGravityAcc-std()-Z", "tBodyAccJerk-mean()-X", "tBodyAccJerk-mean()-Y", "tBodyAccJerk-mean()-Z", "tBodyAccJerk-std()-X", "tBodyAccJerk-std()-Y", "tBodyAccJerk-std()-Z", "tBodyGyro-mean()-X", "tBodyGyro-mean()-Y", "tBodyGyro-mean()-Z", "tBodyGyro-std()-X", "tBodyGyro-std()-Y", "tBodyGyro-std()-Z", "tBodyGyroJerk-mean()-X", "tBodyGyroJerk-mean()-Y", "tBodyGyroJerk-mean()-Z", "tBodyGyroJerk-std()-X", "tBodyGyroJerk-std()-Y", "tBodyGyroJerk-std()-Z", "tBodyAccMag-mean()", "tBodyAccMag-std()", "tGravityAccMag-mean()", "tGravityAccMag-std()", "tBodyAccJerkMag-mean()", "tBodyAccJerkMag-std()", "tBodyGyroMag-mean()", "tBodyGyroMag-std()", "tBodyGyroJerkMag-mean()", "tBodyGyroJerkMag-std()", "fBodyAcc-mean()-X", "fBodyAcc-mean()-Y", "fBodyAcc-mean()-Z", "fBodyAcc-std()-X", "fBodyAcc-std()-Y", "fBodyAcc-std()-Z", "fBodyAccJerk-mean()-X", "fBodyAccJerk-mean()-Y", "fBodyAccJerk-mean()-Z", "fBodyAccJerk-std()-X", "fBodyAccJerk-std()-Y", "fBodyAccJerk-std()-Z", "fBodyGyro-mean()-X", "fBodyGyro-mean()-Y", "fBodyGyro-mean()-Z", "fBodyGyro-std()-X", "fBodyGyro-std()-Y", "fBodyGyro-std()-Z", "fBodyAccMag-mean()", "fBodyAccMag-std()", "fBodyBodyAccJerkMag-mean()", "fBodyBodyAccJerkMag-std()", "fBodyBodyGyroMag-mean()", "fBodyBodyGyroMag-std()", "fBodyBodyGyroJerkMag-mean()", "fBodyBodyGyroJerkMag-std()")

##Activities Vector

c(1, 2, 3, 4, 5, 6)

##Activity Names Vector

c("WALKING", "WALKING_UPSTAIRS", "WALKING_DOWNSTAIRS", "SITTING", "STANDING", "LAYING")

