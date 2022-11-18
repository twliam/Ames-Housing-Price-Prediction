# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2: Ames Housing Data and Kaggle Challenge

### Liam Ting Wei, SG-DSI33

### Problem Statement
The year is 2011. As a member of the data team at an established real estate company located in Ames you have been tasked with creating a regression model that is able to predict property prices. This predictive model should serve the property agents in your company well by allowing them to provide fair valuations to clients as well as identify houses that will net them more commissions. These valuations are however, worthless if inaccurate, so there is an accuracy requirement of R2 > 0.75.

As part of the process, you are also required to give some insights regarding factors that influence the selling price of a house as well as make recommendations based on these. 

### Background
With a population of around 60,000, Ames is the 9th biggest city in Iowa. It has a humid, continental climate, complete with four seasons. Summers are hot (up to 74 degrees Fahrenheit in July), and winters are cold (down to 20.4 degrees Fahrenheit in Jan). Households in Ames own 2 cars on average. 

source: [Data USA](https://datausa.io/profile/geo/ames-ia/)

### Summary
The ames housing dataset contains 80 features and 1 target variable. A filter method was used to select features and build 3 regression models for evaluation. Both regularized regression models Ridge and Lasso performed significantly better than both the null model and vanilla linear regression. **Lasso regression** was ultimately selected as the production model for its reduced complexity and ease of interpretability. Further, it met our accuracy requirement of an R2 score of > 75%.

Living area above grade, overall quality, and garage area have the largest positive contributions to changes in predicted sale price, even more so than lot area. Some neighborhoods have a relatively stronger positive impact on sale price while some had negative relationships. The feature that had the greatest negative effect on sale price is house age.

*Model obtained a Kaggle Score of 26373 (RMSE)*

### Conclusions and Recommendations

Recommendations for agents to identify higher value houses:
1. Location is important, as always. houses in good neighborhoods sell for more. 
2. Use built-up size as a gauge rather than total lot size. Having more livable area above ground or a larger garage seems to impact selling price more than just how big the lot area is.
3. Look out for the overall quality of materials and finishing of a house.  

Recommendations to increase house value before listing:
1. Improving the overall quality of the house just prior to selling might be feasible, as finishings such as painting, flooring, plastering or minor woodwork can be done on short notice.
2. Upgrading your kitchen is another viable option.
3. Some of the stronger factors that impact sale prices (built-up area, garage size) may be costly and time consuming to pursue. May not be worth your while.

### Future Direction
Track if the use of the insights above help agents not just in fair valuation and increasing value of properties but also in closing their clients as well. In some instances, selling price is not the only target. Closing is as important.

### Data
Two datasets,`train` and `test`, are obtained from the Ames Assessor's Office and provided for analysis and modelling. Both datasets are a record of sales for residential properties sold in Ames, Iowa from 2006 to 2010.
* [`train.csv`](./data/train.csv): Contains both features and target
* [`test.csv`](./data/test.csv): Contains only the features without target
