# Happiness-Prediction-Project
**A statistical learning approach to learning different factors that affect the happiness of a population and predicting a happiness score.**

## Introduction
This project is a comprehensive statistical analysis aimed at understanding the diverse factors influencing the happiness levels within populations worldwide. 
Happiness, often regarded as a subjective well-being measure, is influenced by a multitude of socioeconomic, cultural, and environmental factors. This project endeavors to explore and model these factors to predict and gain insights into the determinants of happiness scores across different regions and nations. Through meticulous data exploration, feature analysis, and predictive modeling, this project seeks to uncover patterns, correlations, and predictive relationships that contribute significantly to happiness levels. 

## Objective
The objectives of this project are:

• **Identify Key Factors:** Investigate and uncover influential factors affecting happiness levels.

• **Develop Predictive Models:** Build a robust and reliable model capable of accurately predicting individual happiness scores based on identified factors.

• **Promote Well-being:** Leverage insights derived from the data analysis and predictive modeling to contribute meaningfully towards improving overall well-being and contentment.

## Dataset
World Happiness Report Dataset is specifically chosen because of its global scope, comprehensive nature, and most importantly, it is freely accessible to the public. This dataset is itself a compilation of survey/interview data from the Gallup World Poll which tracks human development worldwide. The poll focuses on understanding the hopes, dreams, and behaviors of people across the globe.

• **GDP per Capita:** It represents the country’s Gross Domestic Product (GDP) divided by its population, reflecting the average economic output per person. It serves as an indicator of a nation’s wealth and standard of living. The GDP per capita is measured in USD and later log scaled for better representation by the WHR dataset.

• **Social Support:** This variable considers factors like family support, community involvement, and access to supportive relationships or simply having someone to count on in times of trouble.

• **Life Expectancy:** Life expectancy represents the average number of years a person is expected to live at birth in a specific country or region. It’s a fundamental indicator of the overall health and well-being of a population.

• **Freedom:** This parameter assesses the degree of political and individual freedom within a society. It includes factors such as civil liberties, political rights, and the absence of oppressive conditions.

• **Generosity:** Generosity reflects the willingness of individuals within a society to engage in charitable acts, donate money or help others without expecting anything in return.

• **Corruption:** Corruption measures the perceived levels of corruption within a country, considering factors like bribery, the integrity of public institutions, and the trustworthiness of governmental bodies.


## Methodology
An exploratory analysis of associated factors for happiness is done. Each factor (or predictor in this case) is studied and compared with each other. Different regression is then modeled to predict the happiness score with varying levels of testing MSE. The predictors were also checked for multicollinearity and appropriate measures to remove the multicollinearity were implemented. 

### Model Tested:
  * Linear Regression Model (**Test MSE: 0.41**)
  * KNN Regression Model (**Test MSE: 0.26**)
  * Lasso Regression (**Test MSE: 0.42**)
  * Ridge Regression (**Test MSE: 0.53**)


## Results
The analysis reveals associations between predictors (Life Expectancy, GDP per capita, Social Support, Freedom) and happiness scores. Corruption shows a negative association, while Generosity displays none. Multicollinearity among predictors affects the stability and accuracy of the linear regression model.

## Tech Stack
* R-Studio
* library(car)
* library(psych)
* library(leaps)
* library(dplyr)
* library(tidyr)
* library(caret)
* library(kknn)
* library(glmnet)
* library(corrplot)
* library(ggplot2)

## References
[1] “Oxford english dictionary. happiness. in oxford english dictionary online..”
https://www.oxfordlearnersdictionaries.com/us/definition/english/happiness?q=happiness,
2022. [Accessed 07-12-2023].

[2] J. F. Helliwell, R. Layard, J. D. Sachs, L. B. Aknin, J.-E. De Neve, and S. Wang, eds., World
Happiness Report 2023 (11th ed.). Sustainable Development Solutions Network, 11 ed., 2023.

[3] SDSN, “Home — worldhappiness.report.” https://worldhappiness.report/. [Accessed 07-12-
2023].

[4] “World Happiness Report — kaggle.com.” https://www.kaggle.com/datasets/unsdsn/world-
happiness. [Accessed 07-12-2023].

[5] “World Happiness Report 2015-2021 — kaggle.com.” https://www.kaggle.com/datasets/mathurinache/wo
happiness-report-20152021. [Accessed 07-12-2023].

[6] “World Happiness Report 2023 — kaggle.com.” https://www.kaggle.com/datasets/ajaypalsinghlo/world-
happiness-report-2023. [Accessed 07-12-2023].

[7] R. Nepal, “World Happiness Dataset (2005 to 2023) — kaggle.com.”
https://www.kaggle.com/datasets/rabinnepal/world-happiness-dataset-2005-to-2023/data,
2023. [Accessed 07-12-2023].

[8] G. James, D. Witten, T. Hastie, and R. Tibshirani, An Introduction to Statistical Learning:
with Applications in R. Springer US, 2021.
