# Getting-and-Cleaning-Data-Course-Project-on-Coursera

# Dataset
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

# Files
### CodeBook.md

The CodeBook.md file provides a comprehensive description of the variables, the dataset, and any transformations or procedures applied to clean the data.

### run_analysis.R

The run_analysis.R script conducts data preparation and follows the 5 steps outlined in the course project’s definition:

1. **Merge Training and Test Sets**:
   - Combines the training and test datasets to create a unified dataset.

2. **Extract Mean and Standard Deviation Measurements**:
   - Extracts only the measurements related to mean and standard deviation for each measurement.

3. **Use Descriptive Activity Names**:
   - Assigns descriptive activity names to label the activities in the dataset.

4. **Appropriately Label Variables**:
   - Provides descriptive variable names to enhance clarity and understanding of the dataset.

5. **Create Independent Tidy Data Set**:
   - Generates a second, independent tidy dataset with the average of each variable for each activity and subject.

### FinalData.txt

FinalData.txt is the exported final dataset resulting from the aforementioned steps, representing a clean, tidy dataset ready for further analysis.
