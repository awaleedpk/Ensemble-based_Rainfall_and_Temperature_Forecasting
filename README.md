# Ensemble-based_Rainfall_and_Temperature_Forecasting
Utilizing a diverse ensemble of 5 ML models, we predict rainfall, min, and max temperatures. Our approach combines classification and regression algorithms for a comprehensive solution. Join us in advancing weather forecasting!
<p style=" text-align: justify;">We are utilizing a diverse ensemble of five distinct machine learning models to conduct predictive analyses on historical dataset pertaining to rainfall, minimum, and maximum temperatures. These models are characterized by their unique methodologies, each possessing specific strengths and capabilities. Our approach entails the incorporation of both classification and regression algorithms, thereby encompassing a comprehensive array of techniques to effectively address the intricacies associated with this multifaceted task. </p>

## Table of Contents
* [Overview of the process](#1)
* [Importing the required libraries](#2)
* [Importing the Weather Dataset](#3)
* [Data Analysis](#4)
    - [Feature Distribution](#41)
    - [EDA](#42)
         - [Average WindSpeed Analysis](#421)
         - [Average Humidity Analysis](#422)
         - [Average Pressure Analysis](#423)
         - [Average Temperature Analysis](#424)
    - [Correlation and Description of the data](#43)
* [Data Preprocessing](#5)
    - [Standardize the Variables](#51)
    - [Transforming Categorical Variables](#52)
* [Rainfall Occurance Prediction](#6)
    - [Training Data and Test Data](#61)
    - [Logistic Regression Model](#62)
    - [KNN Classification Model](#63)
    - [Decision Tree Classification Model](#64)
    - [SVM Classification Model](#65)
    - [Random Forest Classification Model](#66)
    - [Ensembled of the above classification models](#67)
    - [Classification Report on Ranfall Occurance Prediction](#68)
* [Rainfall Amount Prediction](#7)
    - [Training Data and Test Data](#71)
    - [Linear Regression](#72)
    - [Random Forest Regression Model](#73)
    - [SVM Regression Model](#74)
    - [Ensembled of the above Regression Models](#75)
    - [Regression report on rainfall amount prediction](#76)
* [Rainfall Occurance Prediction](#8)
    - [Training Data and Test Data](#81)
    - [Linear Regression](#82)
    - [Random Forest Regression Model](#83)
    - [SVM Regression Model](#84)
    - [Ensembled of the above Regression Models](#85)
    - [Regression report on average temperature prediction](#86)
 


In terms of classifying weather or not rainfall will occur, we will be utilizing-
> 1. Logistic Regression
> 2. Decision Tree Classification
> 3. Random Forest Classification
> 4. K-Nearest Neighbors
> 5. Support Vector Classifier

Furthermore, In terms of predicting rainfall amount or average temperature of a day, our regression-based algorithms will include-
> 1. Linear Regression
> 2. Random Forest Regression
> 3. Support Vector Regression

<b>Ensemble Classifier Regressor:</b> <br>
<p style="text-align: justify;">To achieve comprehensive predictions, our methodology also involves an ensemble classifier. The ensemble classifier operates on a principle of consensus and voting, embodying a collective wisdom that transcends the limitations of any single model. As the classifiers generate their independent forecasts, the ensemble classifier amalgamates these predictions, leading to a dynamic and balanced output that represents the collective insight of the entire ensemble. Specifically, the ensemble classifier will make predictions about the occurrence of rainfall based on historical data patterns. This aggregated result is achieved through intricate mechanisms that
prioritize reliability, accuracy, and robustness. By cultivating harmony among the classifiers, the ensemble classifier fortifies its predictive ability and diminishes the influence of any potential outliers or biases present in the individual models. </p>

We will evaluate our models using:

> 1.  Accuracy Score
> 2.  F1-Score
> 3.  Mean Absolute Error
> 4.  Mean Squared Error

Finally, we will use models to generate the report displaying the accuracy scores.

<a id="2"></a>

> Indented block


# 2. Importing the required libraries
Here, required Python packages have been imported for the analysis.

- The **pandas**, **numpy** packages are required for basic analysis.
- The **matplotlib**, **seaborn** packages are used for visualization purpose.
- The **sklearn** package is used for importing ML models for classification and regression.

<a id="3"></a>
# 3. Importing the Weather Dataset
<a id="4"></a>
# 4. Data Analysis
## 4.1. Feature Distribution
<a id="41"></a>
