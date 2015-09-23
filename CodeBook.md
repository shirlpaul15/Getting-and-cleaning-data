
Original (raw) Data from UCI Machine Learning Repository


Involves working with database Human Activity Recognition built from the recordings of 30 subjects performing activities of daily living (ADL) while carrying a waist-mounted smartphone Samsung Galaxy S2 with embedded inertial sensors.

Original data collected from the smartphones accelerometer and gyroscope 3-axial raw signals, further processed using various signal processing techniques resulting in a measurement vector with 561 features.


For detailed description of the original dataset, refer to README.txt and features_info.txt bundeled with the original data set zip archive. The original data set is split into training and test sets where each partition consists of three files that contain

the measurements from the accelerometer and gyroscope
the labels for activity
the subject identifiers



Tidy Data

Contains aggregated mean values of all mean and standard deviation values from original data set grouped by activity and subject, resulting in a total of 180 records.



More used Attribute Information:

For each activity in Tidy Data is provided:

Activity Label : (One of 6 different Activities)

--> Laying 
--> Sitting 
--> Standing 
--> Walking 
--> WALKING_DOWNSTAIRS
--> WALKING_UPSTAIRS

Experiment carried out by  (30 different subjects, IDs ranging from {1,2,3,...,30})


79 features with the


--> Mean of Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
--> Mean of Triaxial Angular velocity from the gyroscope.
--> numerical value ranging in [-1,1]



VARIABLE NAME :

tbodyacc.mean.x
tbodyacc.mean.y
tbodyacc.mean.z
tbodyacc.std.x
tbodyacc.std.y
tbodyacc.std.z
tgravityacc.mean.x
tgravityacc.mean.y
tgravityacc.mean.z
tgravityacc.std.x
tgravityacc.std.y
tgravityacc.std.z
tbodyaccjerk.mean.x
tbodyaccjerk.mean.y
tbodyaccjerk.mean.z
tbodyaccjerk.std.x
tbodyaccjerk.std.y
tbodyaccjerk.std.z
tbodygyro.mean.x
tbodygyro.mean.y
tbodygyro.mean.z
tbodygyro.std.x
tbodygyro.std.y
tbodygyro.std.z
tbodygyrojerk.mean.x
tbodygyrojerk.mean.y
tbodygyrojerk.mean.z
tbodygyrojerk.std.x
tbodygyrojerk.std.y
tbodygyrojerk.std.z
tbodyaccmag.mean
tbodyaccmag.std
tgravityaccmag.mean
tgravityaccmag.std
tbodyaccjerkmag.mean
tbodyaccjerkmag.std
tbodygyromag.mean
tbodygyromag.std
tbodygyrojerkmag.mean
tbodygyrojerkmag.std
fbodyacc.mean.x
fbodyacc.mean.y
fbodyacc.mean.z
fbodyacc.std.x
fbodyacc.std.y
fbodyacc.std.z
fbodyacc.mean.freq.x
fbodyacc.mean.freq.y
fbodyacc.mean.freq.z
fbodyaccjerk.mean.x
fbodyaccjerk.mean.y
fbodyaccjerk.mean.z
fbodyaccjerk.std.x
fbodyaccjerk.std.y
fbodyaccjerk.std.z
fbodyaccjerk.mean.freq.x
fbodyaccjerk.mean.freq.y
fbodyaccjerk.mean.freq.z
fbodygyro.mean.x
fbodygyro.mean.y
fbodygyro.mean.z
fbodygyro.std.x
fbodygyro.std.y
fbodygyro.std.z
fbodygyro.mean.freq.x
fbodygyro.mean.freq.y
fbodygyro.mean.freq.z
fbodyaccmag.mean
fbodyaccmag.std
fbodyaccmag.mean.freq
fbodybodyaccjerkmag.mean
fbodybodyaccjerkmag.std
fbodybodyaccjerkmag.mean.freq
fbodybodygyromag.mean
fbodybodygyromag.std
fbodybodygyromag.mean.freq
fbodybodygyrojerkmag.mean
fbodybodygyrojerkmag.std
fbodybodygyrojerkmag.mean.freq
activity
subject
