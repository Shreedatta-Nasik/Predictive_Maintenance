# Predictive Maintenance of CMAPSS dataset
 CMAPSS dataset is public dataset released by NASA and contains the sensor reading of turbofan engine, their settings and their remaining useful life. The dataset can be downloaded and it's metadata can be found [here](https://data.nasa.gov/Aerospace/CMAPSS-Jet-Engine-Simulated-Data/ff5v-kuh6/about_data)
 This project is inspire from [Koen Peters](https://github.com/kpeters/exploring-nasas-turbofan-dataset/tree/master) who has done an excellent job in exploring this dataset.
 ## Approaches
  I have mainly used FD001 data in my notebooks and i have considered three methods. They are:
  ### Linear Regression 
This method provided me with the best value for the considered metrics as we are predicting a single variable which is RUL (Remaining Useful Life) due EDA I have modified the dataset to get a better result. 
The modification is explained in the notebook itself.
  ### LSTM
I used LSTM because it was a time series data but it did not provide me with satisfying result. I used exponential smothing on top of the modification.
  ### RBM+LSTM
I refered a [research](Remaining Useful Life Predictions for Turbofan Engine Degradation Using Semi-Supervised Deep Architecture) paper and tried to recreate the model that was explained in the published paper. It also did not provide me with a satifying result
