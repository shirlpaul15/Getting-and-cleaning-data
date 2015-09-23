# Getting-and-cleaning-data

This repository contains the code for Coursera Project "Getting and cleaning data".

The Project being worked upon is "Human Activity Recognition using smartphones"

The following belows explains the functionality of the the code and their respective functions 

IF the following files are not present the following function : DownloadDataSet(url)

Checks if the files exist in the directory , if the following files is not present it will create a folder called "data"
and downloads the file and unzip it for you.


1. Loading test sets and Merging it :

LoadMergeData ()

Based on the assignment both training and test data sets shall be merged. Mainly because of the fact that they reside in different subfolders, the script addresses this while concatenating the common path with the individual subfolder and filenames into global value "path". Load the main file X_train.txt (resp. X_test.txt) into a data frame train.dat (resp. test.dat) then append the Y_train.txt( resp. Y_test.txt) and subject_train.txt(resp. subject_test.txt) to the data frames using read.csv() Once all measurements are loaded, the two data frames train.dat and test.dat can be merged into a single data frame

return result


2. Selecting Required variables 

Function: ExtractData(df)

Assignment truly specifies only the features that contain mean and standard deviation are in scope. Read the file features.txt into a global data frame called "features" using read.csv(). Perform a regex search for strings containing "-mean" or "-std" on the features list and store the result in a global vector called cols.in.scope Therfore, the features in scope are given and the resulting vector can be used to reduce DF "feature" To be able to reduce the DF "Data" add the columns ID for variable "activity" and "subject" to the vector col.in.scope because they need to be kept for later aggregation. Once that's done the col.in.scope vector can be used to remove the obsolete columns out of the input data frame.

return result


3. Use Descriptive activity names (Script performs the following after step 4.)

Function: SetActivityNames(df)

The activity labels are declared in the file activity_labels.txt. Load file into a DF "activity.Labels" using read.csv(). Loop through input data frame and replace activity IDs with their matching lables. return result


4. Descriptive Variable name to name the data set

Function: DescriptiveVariables(df)

Alter the variable names with the use of gsub() function. For better readability and the author choose to make following replacements (following the Rguide):

substitute "-mean" with ".mean"
substitute "-std" with ".std"
substitute "-meanFreq()" with ".mean.freq"
substitute "-" with "."
remove "()"
convert upper to lower case
return result



5. Creating Data set Tidy

Function: MakeTidy(df)

Declare the variable activity and subject as noiminal data with R function as.factor() To avoid errors on aggregation use subset of DF Data (the columns containing numeric data, which are all except the last two columns activity and subject) Then aggregate by grouping on "activity" and "subject" calculating the mean for each (numeric) variable and return the result.


Finally,

Write global DF Tidy.Data into the file tidy.txt using tabs as separators and avoid line numbers.


More details for results and variables on CodeBook.md
