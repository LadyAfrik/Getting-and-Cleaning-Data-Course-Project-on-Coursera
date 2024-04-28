The run_analysis.R script conducts data preparation followed by the 7 steps:

1. **Download the dataset**: The dataset is downloaded and extracted into a folder named "UCI HAR Dataset".

2. **Assign each data to variables**:
   - `features` contains feature descriptions from features.txt.
   - `activities` contains activity labels and their corresponding codes from activity_labels.txt.
   - `subject_test` contains test data of volunteer test subjects.
   - `x_test` contains recorded features test data.
   - `y_test` contains test data of activity code labels.
   - `subject_train` contains train data of volunteer subjects.
   - `x_train` contains recorded features train data.
   - `y_train` contains train data of activity code labels.

3. **Merge the training and test sets**: 
   - `X`, `Y`, and `Subject` are created by merging corresponding datasets using `rbind()` function.
   - `Merged_Data` is created by merging `Subject`, `Y`, and `X` using `cbind()` function.

4. **Extract measurements on mean and standard deviation**:
   - `TidyData` is created by subsetting `Merged_Data`, selecting only relevant columns.

5. **Use descriptive activity names**:
   - Activity codes in the `TidyData` are replaced with corresponding activity names from the `activities` variable.

6. **Label the dataset with descriptive variable names**:
   - Column names in `TidyData` are appropriately renamed for clarity and consistency.

7. **Create a second tidy data set**:
   - `FinalData` is created by summarizing `TidyData` to calculate the means of each variable for each activity and subject.
   - The result is exported to a file named FinalData.txt.

This script ensures data cleanliness, clarity, and consistency, facilitating further analysis.
