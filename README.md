# Music-Recommendation-System
KKBOX music recommendation system   
Detailed information can be found at: https://www.kaggle.com/c/kkbox-music-recommendation-challenge

## This project is for MAFS6010S
The main purpose of this project is for to build a Music Recommendation System using a data set with over 7 million records provided KKBOX, Asia’s leading music streaming service. The system is expected to predict the chance of users re-listening to the specific songs within a month. Detailed procedure and results are provided on the `Report.pdf`.


        
## Data set (introduction to 2 subfolders)
### DataProcessing folder 
This folder saves two notebooks to process the data.   
`DataProcessing.ipynb`: This file combines records, song information, user information all together. 

`FeatureData.ipynb`: This file includes extracting useful information from song informaton, song extra information, and user information. This notebook adds 10 more features and encodes all the categorical predictors.

### CompleteDataSet folder    
This folder saves raw data from KKBOX, as well as the processed data.      
1.*train_data.csv* combines records, song information, user information all together. This file is an export from   `DataProcessing.ipynb`.   
    
2.*processed_train_1.csv* is an export from `FeatureData.ipynb`     
   
3.*FinalEncodedTrain.csv* further processes with the added features. This file is an export from `FeatureData.ipynb`   
   
Same applies to 3 other files for testing data.   
   
   
## Models
All the models are run and evaluated solely based on training data set provided by KKBOX. The training set is then divided into a training subset, a validation subset and a testing subset.
   
1.`Logistic Regression-orignial data.ipynb`: Logistic regression model fit with original data (no additional features).  
2.`Logistic_FeaturedData.ipynb`: Logistic regression model fit with featured data.  
3.`LightGBM.ipynb`:  Light gradient boosting machine with featured data.  
4.`RandomForest.ipynb`: Random Forest model with featured data.    
5.`KNN.ipynb`: KNN with featured data.


