# Data Science Final Project

### Jasmine Jha - jj1073, David Gentili - dag162, Duana Blach - db1605, Maddie Dimarco - msd150


## Overview 

For this project, we aim to predict Multidimensional Poverty Index (MPI) at a block level in the city of Medellin using Geospatial data. In this attempt, we tried to replicate the paper "Predicting Multidimensional Poverty with Machine Learning Algorithms: An Open Data Source Approach Using Spatial Data" by Guberney Muñetón-Santa and Luis Carlos Manrique-Ruiz. The MPI in this data set will be used as the outcome of interest in our analysis. 

## Data Set

To do this, you can download the two primary data sets:
1. Multidimensional Poverty Index (MPI) calculated at the street block level for the city of Medellin from the National Department of Statistics of Colombia (DANE), available in: https://geoportal.dane.gov.co/visipm/. The MPI in this data set will be used as the outcome of interest in our analysis.
2. As explanatory variables we will attempt to use the distance from each block to public infrastructure in the city. This information is downloaded from Open Street Map (OSM) using the library(osmdata).

To run the analysis, you will use the "data_wrangling_medellin.qmd" in the repository for this project. This will take several hours to run fully, as it requires significant computational power. Once you export the final data set as a csv, you can shift to the index.qmd file. We kept the data wrangling separate from the main analysis file to ensure the viewer could start by combining the data sets before they move to the full analysis. (Additional narrative on the data wrangling is provided within the index.qmd file).


## Supevised Machine Learning - Regression & Classification

We start with exploratory data analysis and continue with supervised machine learning for both Regression and Classification models. For this first part, we aim to predict Multidimensional Poverty at a block level in the city of Medellin using Geospatial data. For the regression, we run the linear regression model, KKN model and random forest, and then we chose the best-fit model with the lowest rmse. The best-fit model in this case is the KNN model on testing data to predict MPI by block level. For the classification model, we ran a KNN model, logsitic model, and decision tree, and then chose the best-fit model with the highest accuracy, which was the KNN model in this case. 


## Steps to replicate

1. Clone this repository to your local machine (git clone on the Terminal), choosing a directory of your preference.
2. Make sure you have R and any necessary packages installed.
3. Open the R.proj file in R Studio.
4. Run the data wrangling code line by line or the entire script. Export the final data set to csv.
5. Run the analysis code line by line or the entire script.
