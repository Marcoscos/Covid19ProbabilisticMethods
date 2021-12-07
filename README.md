# Covid19ProbabilisticMethods
This repo contains a project whose objective is to forecast the total number of vaccinations in each country based on the World Bank's Covid-19 dataset, using probabilistic models.

Probabilistic models are part of what is called "Bayesian" methodologies, as opposed to the regular machine learning or "Frequentist" methodologies. These methods focus on acknowledging and quantifying both what is known and what is unknown. The probabilistic methods approximate (physical) processes to probability distributions and by understanding the underlying processes they are able to make predictions and quantify uncertainty.

About the project itself, it consists of the following stages: preprocessing, exploratory data analysis, data preparation, modelling and evaluation.
It was a group project which was the focus of the course 42186 - Model-Based Machine Learning taught at the Technical University of Denmark.

The course is centered around the modelling of probabilistic methods, and so is the project. The main file, "Final_Vaccination Prediction.ipynb" consists mostly of iterations of several models, starting from a rather simple AR(1), to an AR(2) with a hierarchical model, somewhat closer to the "ideal" model:

![image](https://user-images.githubusercontent.com/72278168/145003850-da5bd220-46b4-42f3-9bd0-3ec7f758c027.png)

Starting with the preprocessing, the dataset is expanded with a bunch of economic, health and education-related indicators about the countries. Thanks to these new indicators of the countries' wellbeing, the different countries are grouped into 4 different clusters. To do this, first the dimensionality of the data is reduced using PCA and with its results the countries are clustered with a KMeans algorithm. 

![image](https://user-images.githubusercontent.com/72278168/145009700-743498d9-ae1b-4c28-ad69-cd5ba6596a49.png)

This chart allows to better understand the similarities between countries on economic, health and education-related indicators. It is expected that countries belonging to the same clusters have similar strategies regarding the vaccination rollout and therefore the predictions should be within the same range.

Having done this the data is prepared and formatted to be able to perform the forecasting. It is prepared with weekly frequency both for the clusters and for the countries.
