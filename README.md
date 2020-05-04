# Machine Learning Final Project
Progress will be posted on this repo. As of May 1st, this is what we have done. 

We will be working on the dataset *Breast Cancer Wisconsin (Diagnostic)*,  updated 4 years ago (Version 2) and posted on Kaggle: 
https://www.kaggle.com/uciml/breast-cancer-wisconsin-data

It can also be found on UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29


## Description of the Data
The dataset is hosted by the University of California Irvine, and was created by the University of Wisconsin’s Dr. William H. Wolberg, W. Nick Street, and Olvi L. Mangasarian. 

The dataset contains 32 attributes from 569 breast cancer patients in Wisconsin dating from around ~1992. Each datapoint is composed of the attributes of the nuclei of a cluster of cells obtained via fine needle aspiration and analyzed under a microscope. 

An observation consists of an ID number, a diagnosis (M or B), mean, standard error, and “worst” (average of the three largest values) for the following: radius (average distances from center to the outside), texture (standard deviation of gray-scale values), perimeter, area, smoothness (variation in length of radius), compactness (perimeter^2 /(area - 1.0)), concavity (severity of concave portions of the contour), concave points (number of concave portions of the contour), symmetry and fractal dimension (coastline approximation" - 1) for a cell nucleus. 

The target variable diagnosis has 212 malignant, and 357 benign. The dataset has no missing values.          


## Motivation/Description
We will use Rmarkdown to determine the type of tumor a breast cancer patient has, malignant (M) or benign (B) by using data procured from biopsy samples of Wisconsin cancer patients in the early 1990s. Our project will also compare the results from K-NN and Naive Bayes to determine which machine learning algorithm is the best for predicting the type of cancer in a small dataset. It will also examine how variable selection affects the error rate for K-NN and Naive Bayes. Another goal is to compare the results from K-NN, Naive Bayes, Linear Discriminant Analysis and Quadratic Discriminant Analysis to determine which machine learning algorithm is the best for predicting the type of cancer in a small dataset. 


## Description of the ML Algorithm
Data exploration and a Chi-square test will be used to determine which variables are predictors for the type of tumor the breast cancer patient has. K-means clustering is used to bin the variables. The optimal k was found using the elbow 
method while also maintaining the minimum number of observations required to run the 
Chi-squared test. Both the elbow method and silhouette method were considered for selecting the
the optimal k. The elbow method was chosen by the contributors, because it created varying bins. 

K-NN and Naive Bayes will be run using all the predictor variables in the dataset. These same algorithms will also run with only the variables that are significant predictors of the type of cancer. The results will be compared to determine if there is a difference between the error rate of using all the variables and the error rate of using only the significant predictors. The error rates will also be examined to determine whether K-NN or Naive Bayes works best at predicting the type of tumor the breast cancer patient has.

## Final Report
Latex report is posted on https://github.com/kellyav/358_Final 


## Contributors: 
@kellyav Alexa Kelly // alexavkelly98@gmail.com

@ryandoesmath Ryan Folks // rfolks92@gmail.com

(@lswarey) Lyndon Swarey // lswarey@gmail.com
