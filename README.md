# Data Science Final Project

### Jasmine Jha - jj1073, David Gentili - dag162, Duana Blach - db1605, Maddie Dimarco - msd150

## Data Set

We get the dataset or Multidimensional Poverty Index (MPI) calculated at the street block level for the city of Medellin from the National Department of Statistics of Colombia. The MPI in this data set will be used as the outcome of interest in our analysis. We worked to create a data set where each block in the city is one row, and the distances from the closest public service (referred to as an amenity) are the columns. The amenities categories used are schools, hospitals, police stations, fire stations, bus stops, and places of worship. Hence, the goal was to have, for each block, one column for each category of amenity, with the distance to the closest one.

## Supevised Machine Learning - Linear Regression

We start with exploratory data analysis and continue with supervised machine learning - Regressions model. For this first part, we aim to predict Multidimensional Poverty at a block level in the city of Medellin using Geospatial data. After we run the linear regression model, KKN model and random forest, we choose the best-fit model with the lowest rmse. The best-fit model in this case is the KNN model on testing data to predict MPI by block level.

## Comparison with Actual and Predicted MPIs

Then using the shape file for the city we add the predicted MPI column to it. Further, we calculate the absolute difference between the actual and predicted MPIs, and use this information to compare the actual MPIs with the predicted MPIs.
