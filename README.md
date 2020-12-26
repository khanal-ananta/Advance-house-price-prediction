# california-house-price-prediction


### The general description of the dataset is as:

download dataset from here https://www.kaggle.com/camnugent/california-housing-prices

    longitude: A measure of how far west a house is; a higher value is farther west

    latitude: A measure of how far north a house is; a higher value is farther north

    housingMedianAge: Median age of a house within a block; a lower number is a newer building

    totalRooms: Total number of rooms within a block

    totalBedrooms: Total number of bedrooms within a block

    population: Total number of people residing within a block

    households: Total number of households, a group of people residing within a home unit, for a block

    medianIncome: Median income for households within a block of houses (measured in tens of 
    thousands of US Dollars)

    medianHouseValue: Median house value for households within a block (measured in US Dollars)

    oceanProximity: Location of the house w.r.t ocean/sea
    
    
### Description of the model buidling process

1) Data cleaning : Missing data analysis is done by replacing missing data with mean.

2) Data analysis and visualization : Data is analyse and visualize by using histogram, scatter plot and heatmap.

3) Handel categorical data : Categorical data is handled by using get dummy variable approach.

4) Split data set : Total data set is splited into train and test data set in the ratio 4:1.

5) Centering and scaling : Centering and scaling is done by using StandardScalar.

6) Build models : Regression is done using Linear regression, Decision tree and xgboost. R2 value is compared among all these regressors.

                 linear regression : 0.6381617983930403
                 decision tree regression : 0.6440459585747119
                 xgboost regression : 0.8290325384571818
                 
                 
7) Hyperparameter optimization : Randomized searchCV with 4 fold cross validation is used to find the optimum values of parameter for xgboost regression.

8) The final value of R2 we get is 0.841819678128336 which is quiet good for this project.


