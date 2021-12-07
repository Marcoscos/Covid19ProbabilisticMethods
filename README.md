# Covid19ProbabilisticMethods
This repo contains a project whose objective is to forecast the total number of vaccinations in each country using probabilistic models, based on the World Bank's Covid-19 dataset.

The project consists of the following stages: preprocessing, exploratory data analysis, data preparation, modelling and evaluation.
This was a group project which was the focus of the course 42186 - Model-Based Machine Learning taught at the Technical University of Denmark.

The course is centered around the modelling of probabilistic methods, and so is the project. The main file, "Final_Vaccination Prediction.ipynb" consists mostly of iterations of several models, starting from a rather simple AR(1), to an AR(2) with a hierarchical model, somewhat closer to the "ideal" model:

![image](https://user-images.githubusercontent.com/72278168/145003850-da5bd220-46b4-42f3-9bd0-3ec7f758c027.png)


About the preprocessing, the dataset is expanded with a bunch of economic, health and education-related indicators about the countries. 
