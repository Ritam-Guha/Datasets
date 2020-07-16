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
** train
** trainLabel
** test
*** testLabel
