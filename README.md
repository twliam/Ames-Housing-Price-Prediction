# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2: Ames Housing Data and Kaggle Challenge

### Liam Ting Wei, SG-DSI33

### Problem Statement
The year is 2011. As a member of the data team at an established real estate company located in Ames you have been tasked with creating a regression model that is able to predict property prices. This predictive model should serve the property agents in your company well by allowing them to provide fair valuations to clients. However, these valuations are worthless if inaccurate, so there is an accuracy requirement of R2 > 0.75.

As part of the process, you are also required to give some insights regarding factors that influence the selling price of a house as well as make recommendations based on these. 

### Background
With a population of around 60,000, Ames is the 9th biggest city in Iowa. It has a humid, continental climate, complete with four seasons. Summers are hot (up to 74 degrees Fahrenheit in July), and winters are cold (down to 20.4 degrees Fahrenheit in Jan). Households in Ames own 2 cars on average. 

source: [Data USA](https://datausa.io/profile/geo/ames-ia/)

### Summary
The ames housing dataset contains 80 features and 1 target variable. A filter method was used to select features and build 3 regression models for evaluation. **Lasso regression** was ultimately selected as the production model for its reduced complexity and ease of interpretability. Further, it met our accuracy requirement of an R2 score of > 75%.
Living area above grade, overall quality, and garage area have the largest positive contributions to changes in predicted sale price. Some neighborhoods have a relatively stronger positive impact on sale price while some had negative relationships. The feature that had the greatest negative effect on sale price is house age.

### Conclusions and Recommendations

Recommendations made to find houses with higher values are as follows:
1. Location is important, choose houses in good neighborhoods.
2. The top 2 factors that impact sale prices are potentially costly and time consuming to pursue. Find houses that have more built-up area and a larger garage.

Recommendations to increase house value:
4. Improving the overall quality of the house just prior to selling might be feasible, as finishings such as painting, flooring, plastering or minor woodwork can be done on short notice.
5. Upgrading your kitchen is another viable option

### Data
Two datasets,`train` and `test`, are obtained from the Ames Assessor's Office and provided for analysis and modelling. Both datasets are a record of sales for residential properties sold in Ames, Iowa from 2006 to 2010.
* [`train.csv`](./data/train.csv): Contains both features and target
* [`test.csv`](./data/test.csv): Contains only the features without target
