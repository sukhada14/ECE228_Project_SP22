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

There are 2 .ipynb files in this repo.
1.ML_methods.ipynb
2.DL_Timeseries_methods.ipynb

## Data
## Code
### In 1.ML_methods.ipynb, 

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

### In 2.DL_Timeseries_methods.ipynb, 

A well documented code for reading the data (crop_type_mapping data in Kenya), training and testing of 3 different deep learning time series
based models is provided.

Step 1: Reading the numpy files and metadata

Step 2: Cleaning the data- removing rows with null values
        
Step 3: Train 3 models (LST, SimpleRNN, GRU) on the 80% training data

Step 4: Visualization for comparative analysis of training loss values for 3 models

Step 5: Test the models on 20% test data


