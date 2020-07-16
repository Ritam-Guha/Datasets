# This sub-repo contains a set of processed UCI datasets

Every folder has two files-
* A .csv file 
* A .mat file

UCI datasets are generally maintained in .dat format which is harder to format.
I have converted the selected set of data into CSV format.

Every csv file has -
* set of features (all the columns except the last one)
* class labels (last column of each dataset)

***csv files are extremely useful and easy to format. Almost all the major programming languages have libraries to work with CSV files***

The structure of the mat file is-
* data
    * train
    * trainLabel
    * test
    * testLabel

***Specifically for MATLAB, I felt the test-train division was a bit difficult. That's why instead of using CSV for MATLAB, I prefer processing the data and storing them in mat files***

The mat files contain data division in 70-30 format (70% training, 30% testing). Validation sets are not provided, I prefer using k-fold cross validation with training data only. So, validation sets are not required at all.
