# Kings-County-Housing-Prediction-Model

![Image](https://media.gettyimages.com/photos/sunset-seattle-picture-id615989790?k=20&m=615989790&s=612x612&w=0&h=Ai9z_Bp8yePIiFy6F5PO0KywqrYLfWW53VYSzL-2pW8=)

**Authors:** Grace Arina, Justin Sohn, Anthony Warren

## Business Problem
---

The goal is to save the new home buyers some time and to help ensure consistency in pricing between new houses on the market and old houses.

The main purpose of this algorithm is predictive, meaning that this model should be able to take in attributes of the King's County dataset that does not yet have a set price, and to predict a good price. The effectiveness of this predictive model will be measured by how well it predicts prices in our test set, where we know what the actual prices were but the model does not.

The secondary purpose of this algorithm is inferential, meaning that the model should be able to tell us something about the relationship between the attributes of a house in King's County and its price.

## Analysis Questions
---

This analysis will seek to answer three questions about the data:

**Question 1**: Which features are most highly correlated with price?

**Question 2**: Which features have the strongest correlations with other predictor variables?

**Question 3**: What combinations of features is the best fit, in terms of predictive power, for a multiple regression model to predict house prices?

## Data
---
The King County Housing Data Set contains information about the price, size, location, condition and other features of houses in the Washington’s King County area.
After data cleaning:
- 21,597 house sales between May 2014 – May 2015
- 21 variables


## Methods
---

After cleaning the data for incorrect/missing values, we dropped the 'id' column as it wouldn't be useful going forward. Next, we've listed out the variables by type (categorical vs continuous) and plotted a corresponding heatmap for all of the non-dropped columns

![Image] Documents/Flatiron/phase_2/Kings-County-Housing-Prediction-Model/Correlation Heat Map.png
<img src="Documents/Flatiron/phase_2/Kings-County-Housing-Prediction-Model/Correlation Heat Map.png" width="250"/>
Next, we then perform a train-test split to train and eventually test a model to see how well it works with the newly obtained test data.

From here, we've obtained our baseline, numeric, and final models

## Results
---
### Seasonal Factor
![image](https://user-images.githubusercontent.com/93217519/148599375-1751e064-299b-448d-a95d-35ea36e2991d.png)
![image](https://user-images.githubusercontent.com/93217519/148599405-8fd635ce-6236-4fcf-804d-469abbe47f15.png)

Average and median sale prices were the highest between April-June, while the opposite is true between November-February


### Geographical Factor
![image](https://user-images.githubusercontent.com/93217519/148599466-f6c8210d-c031-4c67-96f6-181bf798d829.png)
Higher Prices:
- Houses between downtown Seattle and  downtown Redmond tend to have higher prices
- Tend to be clustered
- Near water area
Lower Prices:
- Tend to be spread out
- Houses in the southern part of King County have lower prices

### Home Quality
![image](https://user-images.githubusercontent.com/93217519/148599579-ed25029c-c593-4405-abb1-d28ada1661ad.png )


### Inferential Model
![image](https://user-images.githubusercontent.com/93217519/148598127-ec091928-1a2c-4642-b20e-bc166b569465.png )

All other factors held constant:
- The further up north in King County the home is located, the higher the price of the home with a coefficient of $141,214 with each increase of latitude
- Each additional square footage of living space in the home is associated with an increase of $249 in price
- Each additional bedroom is associated with a decrease of $46,098 in the price of a home
- Each additional bathroom is associated with an increase of $10,629 in the price of a home
- The age of the home, yr_built, has a negative association with price with a decrease of $3,392 per year


## Model
![image](https://user-images.githubusercontent.com/93217519/148600151-fefe9644-17e4-493d-a4bb-debc0867f659.png)

## Recommendations
---
Together, square footage, grade and bathrooms are the best predictors of a house's price in King County. Homeowners who are interested in selling their homes at a higher price should focus on expanding square footage and improving the quality of construction. When expanding square footage, homeowners should consider building additional bathrooms, as this analysis suggests that number of bathrooms is positively related to price.

## Conclusion
---
