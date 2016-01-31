<h1>Introduction</h1>
The script run_analysis.Rperforms the 5 steps described in the course project's definition.


<li>First, all the similar data is merged using the rbind() function. By similar, we address those files having the same number 
of columns and referring to the same entities.</li>
<li>Then, only those columns with the mean and standard deviation measures are taken from the whole dataset. </li>
<li>After extracting these columns, they are given the correct names, taken from features.txt.</li>
<li>As activity data is addressed with values 1:6, we take the activity names and IDs from activity_labels.txt and 
they are substituted in the dataset.</li>
<li>On the whole dataset, those columns with vague column names are corrected.</li>
<li>Finally, we generate a new dataset with all the average measures for each subject and activity type 
(30 subjects * 6 activities = 180 rows). The output file is called final_tidy-dataset.txt, and uploaded to this repository.</li>


<h1>Variables</h1>
<li>x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.</li>
<li>X_dataset, y_dataset and subject_dataset merge the previous datasets to further analysis.</li>
<li>features contains the correct names for the X_filtered_dataset dataset, which are applied to the column names stored in feature_selected_columns, 
a numeric vector used to extract the desired data.</li>
<li>A similar approach is taken with activity names through the activities variable.</li>
<li>activity_labels merges x_data, y_data and subject_data in a big dataset.</li>
<li>Finally, tidy_dataset contains the relevant averages which will be later stored in a .txt file. </li>
