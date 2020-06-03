# Music-Recommendation-System
KKBOX music recommendation system   
Detailed information can be found at: https://www.kaggle.com/c/kkbox-music-recommendation-challenge    
Data set can be downloaded at: https://www.kaggle.com/c/kkbox-music-recommendation-challenge/data


## This project is for MAFS6010S
The main purpose of this project is for to build a Music Recommendation System using a data set with over 7 million records provided KKBOX, Asia’s leading music streaming service. The system is expected to predict the chance of users re-listening to the specific songs within a month. Detailed procedure and results are provided on the `Report.pdf`.


        
## DataProcessing folder 
This folder saves two notebooks to process the data. Both take the 5 data sets provided by KKBOX as input.   
`DataProcessing.ipynb`: This file combines records, song information, user information all together. The export is *train_data.csv*, which will be used in the first model--`Logistic Regression-orignial data.ipynb`. 

`FeatureData.ipynb`: This file includes extracting useful information from song informaton, song extra information, and user information. This notebook adds 10 more features and encodes all the categorical predictors.The exports are *processed_train_1.csv*(Not encoded) and *FinalEncodedTrain.csv*(encoded). The later file will be used throughout model 2 to model 5.  

Although both files process the testing data in the same way, this project only uses the training data set provided by KKBOX. The original training set is  training set(x_train) and a testing set(x_test) with the later being 20 percent   
   
   
## Models
All the models are run and evaluated solely based on training data set provided by KKBOX. The training set is then divided into a training subset, a validation subset and a testing subset.
   
1.`Logistic Regression-orignial data.ipynb`: Logistic regression model fit with original data (no additional features).  
2.`Logistic_FeaturedData.ipynb`: Logistic regression model fit with featured data.  
3.`LightGBM.ipynb`:  Light gradient boosting machine with featured data.  
4.`RandomForest.ipynb`: Random Forest model with featured data.    
5.`KNN.ipynb`: KNN with featured data.


