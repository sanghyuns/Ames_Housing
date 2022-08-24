# Project 2 - Ames Housing Data and Kaggle Challenge

## Introduction & Problem Statement

There are many factors that influence the final price of a house. With enough data, there is a way to to create a linear regression model to try to finalize which features of a home help predict the final price of a home most accurately.

Our problem statement is as follows:
How can we use a linear regression model to best predict house sale prices?

With this information, it is my hope that property owners are properly able to make decisions to maximize the value of their homes.

The dataset is from Ames, Iowa. It contained over 2000 housing unit observations with more than 80 features that were observed. My goal for this project was to create a highly accurate model that can be generalized to other datasets. I will be measuring the performance of my linear regression model with root mean squared error (RMSE), which is the differences between values predicted by the model and the values actually observed.

## Conclusions 

Based off of the R squared scores from the project, the lasso model seems to be the most accurate when it comes to predicting the sale price of homes.
The R2/RMSE values of the ridge model are as follows:

Training R2(Lasso)  0.9026161395948707
Testing R2(Lasso): 0.8868392505264129

Training RMSE(Lasso): 24359.00577454118
Testing RMSE(Lasso): 27546.399776496703


This is a huge improvement of the baseline RMSE that was calculated using the mean of all sale prices as predictions. This model seems to be much more generalizable and more accurate with a 90.26% R2 score.

The top 5 predictors of sale price in our model turned out to be the total basement square feet, overall quality, total rooms above ground, and basement type 1 finished square feet. It is good to note that features that include square feet cannot be improved much more than it is due to spacial limitations, so it would be better to look at features that could be improved. There are other good predictors of sale price such as neighborhoods like Northridge Heights and StoneBrook.

## Recommendations

Based on our model, any homeowner that is looking to maximize their home value could do the following

    - Improve the overall material and finish of the house
    - Improve the kitchen quality
    - Improve external quality of the house
    - If possible, improve garage size to fit more cars
    
It is also important to note that since this model was based on the city of Ames, it will be hard to generalize to other cities due to possibility of severe differences of features.

## Data Dictionary
A detailed data dictionary can be found [here](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt).
