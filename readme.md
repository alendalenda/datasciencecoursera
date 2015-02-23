
Hello, my friend!

 Naming the columns
================
 I added the names of the columns contained in the features.txt file
 
 Extracting mean and std measurements
================
 To Extract only the measurements on the mean and standard deviation for each measurement I scanned all the names of the variables and removed the columns of the dataset when the columns neither contained "mean" nor "std"
 
 Use descriptive activity names
================
 To use descriptive activity names to name the activities in the data set I first loaded the data of 'activity_labels.txt', the made a join on activity id and then removed the useless activity id columns
 
 Descriptive variable names
================
 To appropriately labels the data set with descriptive variable names I removed '()' and '-' charaters in the variable names and used uppercase to have 'Mean' instead of 'mean' and 'Std' instead of 'std'
 
 Tidy data set
================
 To creates a second, independent tidy data set I used ddply form plyr package to group by columns Subject.id and Activity.Name and apply the mean to the other variables.
 I then recorded the tidy set in the 'my_tidy_data_set.txt' file.
