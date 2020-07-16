# This sub-repo contains a set of pre-processed UCI datasets

Every folder has two files-
* A .csv file 
* A .mat file

UCI datasets are generally maintained in .dat format which are harder to format.
I have converted the selected set of data into csv format.

Every csv file has -
* set of features (all the columns except the last one)
* class labels (last column of each dataset)

**csv files are extremely useful and easy to format. Almost all the major programming languages have libraries to work with csv files**

The structure of the mat file is-
* data
    * train
    * trainLabel
    * test
    * testLabel
    
e.g. Suppose I want to get the data for BreastCancer. Then the steps are:
* dataset = 'BreastCancer';
* data = importdata(strcat('Data/',dataset,'/',dataset,'_data.mat'));
* x = data.train;
* t = data.trainLabel;
* x2 = data.test;
* t2 = data.testLabel;


***Specifically for MATLAB, I feel that the test-train division is a bit difficult. That's why instead of using csv for MATLAB, I prefer processing the data and storing them in mat files***

The mat files contain data division in 70-30 format (70% training, 30% testing). Validation sets are not provided, I prefer using k-fold cross validation with training data only. So, validation sets are not required at all.

Till now, this sub-repo contains following pre-processed UCI datasets:
- Arrhythmia
- BreastCancer
- BreastEW
- CongressEW
- Exactly
- Exactly2
- Glass
- HeartEW
- Hill-valley
- Horse
- Ionosphere
- KrVsKpEW
- Lymphography
- Madelon
- M-of-n
- Monk1
- Monk2
- Monk3
- PenglungEW
- Sonar
- Soybean-small
- SpectEW
- Tic-tac-toe
- Vote
- WaveformEW
- Wine
- Zoo
