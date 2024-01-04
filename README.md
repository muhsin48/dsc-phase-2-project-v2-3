# **KING COUNTY PROPERTY SALES ANALYSIS**

**Authors** Immaculate Mwendwa, Shalom Irungu, Stephen Kariuki, Stella Ndegwa, Muhsin Ahmed and Joan Wambua.

## Project Overview

### Business Problem

King County, with a population of 2.252 million, is witnessing rapid growth in its housing market due to strong demand and limited supply, resulting in a fiercely competitive environment. The population increase, driven by the influx of new employees and rising wages for higher-income households, has contributed to some of the nation's fastest-growing house prices. The housing crisis is primarily fueled by supply and demand imbalances. As data scientists, our focus is on offering valuable advice to homeowners and real estate developers in King County, guiding them on how specific home features can impact the estimated value of their properties.

The objectives for this project include:

* To **Develop a model that will assist home buyers and home sellers identify attributes that influence the prices of houses.**
* To **Develop regression models that will guide the real eatate agencies on pricing.**
* To **Determine features that have the biggest impact on the sale price of a house and by how much.**

### The Data

The data we use in this project is the King County House Sales dataset which covers property sales from 2014 to 2015, comprising of 21,420 records with details on home features like bedroom count and room sizes.

## Data Preparation

We applied appropriate preprocessing methods to our tabular data in order to set it up for sucessful statistical analysis. This included handling missing values, handling categorical data and handling outliers. We also performed feature engineering as part of this preprocessing.

## Exploratory Data Analysis

To understand the relationship between our independent variables and the dependent variable (Price), we delved into the following areas:
* Independent variables and their correlation with each other and price.
* Independent variables with a significant correlation with price.
* Featrues that exhibit multicollinearity together.

## Modeling

We constructed our baseline model utilizing sqft_living due to its highest correlation with Price. Subsequently, we employed an iterative approach, engaging in the construction of various models through a systematic and incremental process, which ultimately led us to the development of our final regression model. Below is an illustration of our final regression model.
![Final Regression Model](<Final Regression Model.png>)

## Regression Results

### Validity of the Model:

Although the model provides an explanation for a substantial portion of the variance in housing prices, there is a recognized need for additional investigation to gain a deeper understanding of the impact of bathrooms and to improve the overall validity of the model.

### Significant Property Features:

Bedrooms, sqft_living, view, condition, and grade emerge as pivotal factors influencing housing prices, presenting indispensable considerations for both prospective buyers and sellers in the real estate market.

### Limitations of the Model:

It's important to acknowledge the model's inherent limitations, and in addressing these constraints, log transformation was implemented to adhere to the assumptions of linearity in the modeling process.

## Recommendations
* Model 5 findings suggest:

1. Prioritize bedrooms, sqft_living, view, condition, and grade for accurate pricing.
2. Enhance property features to elevate grade and communicate financial gains.
3. Address bathroom impact inconsistency by refining variables.
4. Promote affordable properties with fewer bedrooms.
5. Leverage scenic views with visuals to attract buyers.
6. Continuously improve the model with additional features and refinements.

## Next Steps
* It is imperative to gather additional data on the homes to ensure a comprehensive examination and avoid overlooking any essential features that could significantly impact the analysis.
* Additionally, considering alternative methodologies beyond regression may be contemplated as a means to fulfill the necessary assumptions and enhance the overall robustness of the analytical approach.

## Necessary Links

* **Jupyter Notebook** [Notebook](<Jupyter Notebook.ipynb>)
* **Presentation** [Non Technical Presentation](<Group 16 Project Presentation.pdf>)

## Repository Structure

├── README.md                           
├── Jupyter Notebook.ipynb   
├── Presentation.pdf  
├── data                                