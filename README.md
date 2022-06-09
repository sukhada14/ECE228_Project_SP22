# ECE228_Project_SP22

The structure of the repo is like:

.
 * Data
   * crop_type_kenya_2017_metadata.csv
   * timeseries
       * 5738 .npy files
 
 * Code
   * 1.ML_methods.ipynb
   * 2.DL_Timeseries_methods.ipynb
 * Report PDF
 * requirements.txt

There are 2 .ipynb files in this repo.
1.ML_methods.ipynb
2.DL_Timeseries_methods.ipynb

## Data
### crop_type_kenya_2017_metadata.csv
It is a metadata file. It contains information about file name,	type of crop, region etc.

### timeseries
This folder has 5738 npy files, each conaining 365 days (1 year) time series data for a field. Each land field is represented by a single
pixel of Sentinel-2 Satellite image. Each pixel has 14 spectral bands. Hence, each image can be represented by timeseries of size (14 x 365).


## Code
### 1.ML_methods.ipynb, 

A well documented code for reading the data (crop_type_mapping data in Kenya), cleaning the data, exploratory data analysis, training \
and testing of 5 different ML models is provided.

Step 1: Reading the numpy files and metadata

Step 2: Cleaning the data- removing rows with null values

Step 3: Data visualization (EDA) 

      -for region-wise crop distribution in Kenya

      -for crop frequency distribution in Kenya

      -for average spectral signatures for 9 crops
        
Step 4: Train 5 ML models on the 80% training data

Step 5: Test the models on 20% test data

Step 6: Visualization for comparative analysis of accuracies

### 2.DL_Timeseries_methods.ipynb, 

A well documented code for reading the data (crop_type_mapping data in Kenya), training and testing of 3 different deep learning time series
based models is provided.

Step 1: Reading the numpy files and metadata

Step 2: Cleaning the data- removing rows with null values
        
Step 3: Train 3 models (LST, SimpleRNN, GRU) on the 80% training data

Step 4: Visualization for comparative analysis of training loss values for 3 models

Step 5: Test the models on 20% test data

## How to run the code
Download the git repository. Install requirements given by requirements.txt. Open both notebooks in a jupyter notebook and click on run all cells to reproduce the results.

