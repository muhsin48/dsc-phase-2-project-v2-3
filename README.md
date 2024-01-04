## Housing Price Prediction Model README
### Overview

This repository contains the implementation and analysis of multiple linear regression models for predicting housing prices. The goal is to explore the relationship between various features and the price of houses.

### Business problem:

The real estate agency aims to provide valuable advice to homeowners on how specific home features will impact the estimated value of their homes. The primary objective is to help homeowners make informed decisions about which features could potentially yield the highest return on investment in terms of increased property value.





### Data:


We have been provided with The King County House Sales dataset which contains property sales between year 2014 - 2015 and 21,420 records of houses sold. Each record in the data set gives features such as number of bedrooms, the size of various rooms in square feet, about the individual homes.


Column descriptions for King County Data Set

*   id - unique identified for a house
*   dateDate - house was sold
*   pricePrice - is prediction target
*   bedroomsNumber - of Bedrooms/House
*   bathroomsNumber - of bathrooms/bedrooms
*   sqft_livingsquare - footage of the home
*   sqft_lotsquare - footage of the lot
*   floorsTotal - floors (levels) in house
*   waterfront - House which has a view to a waterfront
*   view - Has been viewed
*   condition - How good the condition is ( Overall )
*   grade - overall grade given to the housing unit, based on King County
*   grading system
*   sqft_above - square footage of house apart from basement
*   sqft_basement - square footage of the basement
*   yr_renovated - Year when house was renovated
*   zipcode - zip
*   yr_built - Built Year
*   lat - Latitude coordinate
*   long - Longitude coordinate
*   sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
*   sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors

















### Objectives
1. Develop a model that will assist home buyers and home sellers identify attributes that influence the prices of houses.

2. Develop regression models that will guide the real eatate agencies on pricing.

3. Determine features that have the biggest impact on the sale price of a house and by how much.






#### Models
Model 1a: Single Predictor - sqft_living
R-squared: 0.493
Interpretation: Approximately 49.3% of the variance in the dependent variable is explained by sqft_living alone.
Model 1b: Single Predictor - Transformed Price
R-squared: 0.483
Interpretation: Around 48.3% of the variance in the log-transformed price is explained by the predictor.

Model 2: All Features
R-squared: 0.499
Interpretation: Including all available predictors improves the explanation of variance compared to Model 1, but it's still relatively modest.
Model 3: Addressing Multicollinearity and Low Correlation
R-squared: 0.560
Adj. R-squared: 0.559
Interpretation: Improved explanation of variance by addressing multicollinearity and low correlation.

Model 4: Baseline and Categorical Variables
R-squared: 0.580
Adj. R-squared: 0.580
Interpretation: Further improvement, especially with the inclusion of categorical variables.

Model 5: More Features, Categorical Data, and Low p-values
R-squared: 0.590
Adj. R-squared: 0.589
Interpretation: Highest explanatory power among the mentioned models.

#### Data Preparation
Here we will check for duplicates and eliminate them if any, check for missing or null values, outliers and decide on the most appropriate method of handling them and also look at the data types and format them to the most appropriate data type that is suitable for our analysis.

Handling missing values

#### Best Model
Model 5 is chosen as the best model due to its higher R-squared value (0.590) and adjusted R-squared value (0.589).

Evaluation
Assumptions of Linear Regression
Linearity: Verified through regression plots.
Normality: Checked using Q-Q plots and histograms of residuals.
Homoscedasticity: Homoscedasticity test p-value: 1.1098177622590325e-60.
Independence: Durbin-Watson Statistic: 1.9744406888716102.
All variables pass the assumptions of linearity, normality, and homoscedasticity.

### Recommendations:
based on findings from our model:

Consider the importance of bedrooms, sqft_living, view, condition, and grade when estimating or predicting housing prices.

Focus on upgrading property features to improve the overall grade. Communicate the potential financial returns associated with higher-grade properties.

Investigate the inconsistency in the impact of bathrooms on pricing. Collect additional data or refine the variable to better capture its significance.

Consider promoting properties with fewer bedrooms for buyers who prioritize cost-effectiveness. Highlight the advantages of smaller bedroom counts in terms of affordability.

Capitalize on properties with better views, incorporating visuals and descriptions that showcase the scenic surroundings to attract potential buyers.

Continuous efforts to improve the model can be made by exploring additional relevant features and refining existing ones.

### Conclusions:
Model Validity:

The model provides a substantial explanation of housing price variance. However, the impact of bathrooms needs further investigation to enhance the model's validity.

Property Features Influence Pricing:

Bedrooms, sqft_living, view, condition, and grade significantly influence housing prices. These features are essential considerations for buyers and sellers.

There are limitations to the model and we used log transformation to meet assupmtions of linearity

### NEXT STEPS

gathering additional data on the homes as there may be key features missing.

methods other than regression could be used to meet assumptions