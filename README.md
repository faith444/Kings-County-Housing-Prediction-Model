# Kings-County-Housing-Prediction-Model

![Image](https://media.gettyimages.com/photos/sunset-seattle-picture-id615989790?k=20&m=615989790&s=612x612&w=0&h=Ai9z_Bp8yePIiFy6F5PO0KywqrYLfWW53VYSzL-2pW8=)

**Authors:** Grace Arina, Justin Sohn, Anthony Warren

Introduction
---

We are a group of data scientists tasked with helping our stakeholders with their business problems. Our stakeholders include new home buyers, home sellers, and folks in the tech industry who are looking at home prices depending on their distance from downtown Seattle & Redmond.

The Business Problem
---

The goal is to save the new home buyers some time and to help ensure consistency in pricing between new houses on the market and old houses, help home sellers determine the best way for them to get the best deal when they sell their home, and to determine whether distance from the downtown areas have an effect on home prices.

The main purpose of this algorithm is predictive, meaning that this model should be able to take in attributes of the King's County dataset that does not yet have a set price, and to predict a good price. The effectiveness of this predictive model will be measured by how well it predicts prices in our test set, where we know what the actual prices were but the model does not.

The secondary purpose of this algorithm is inferential, meaning that the model should be able to tell us something about the relationship between the attributes of a house in King's County and its price.

Analysis Questions
---

This analysis will seek to answer three questions about the data:

**Question 1**: Which features are most highly correlated with price?

**Question 2**: Which features have the strongest correlations with other predictor variables?

**Question 3**: What combinations of features is the best fit, in terms of predictive power, for a multiple regression model to predict house prices?

Data
---

We've used housing data from the King County dataset, which has records on houses sold from May 2014 to May 2015. 

Methods
---

After cleaning the data for incorrect/missing values, we dropped the 'id' column as it wouldn't be useful going forward. Next, we've listed out the variables by type (categorical vs continuous) and plotted a corresponding heatmap for all of the non-dropped columns.

![Image](<insert heatmap here>)

Next, we then perform a train-test split to train and eventually test a model to see how well it works with the newly obtained test data.

From here, we've obtained our baseline, numeric, and final models.

Results
---

After building our final model, we've obtained the following:

![Image](https://github.com/grace-arina/Kings-County-Housing-Prediction-Model/blob/main/data/Inferential_Model.jpg)

What this translates to is that, according to our model, all other things held constant, for each 1 degree increase in latitude, the price of the home rose by $141,214. With the same assumptions, each 1 unit increase in square footage will raise home prices by $249.

![Image](https://github.com/grace-arina/Kings-County-Housing-Prediction-Model/blob/main/data/R_Squared_Final.jpg)
![Image](https://github.com/grace-arina/Kings-County-Housing-Prediction-Model/blob/main/data/RMSE_Final.jpg)

These two graphs capture our R-Squared of 80.2%, meaning that our model captures 80.2% of the variance in price, and our Root Mean Squared Error of $164,842, meaning that our model is only off by $164,842 in regards to predicting home prices in King County.

![Image](https://github.com/grace-arina/Kings-County-Housing-Prediction-Model/blob/main/data/A_M_Home_Price.jpg)
![Image](https://github.com/grace-arina/Kings-County-Housing-Prediction-Model/blob/main/data/House_Sale_Final.jpg)

From here, we've found that the time of year affects the home prices across average, median, and total home sales.

![Image](https://github.com/grace-arina/Kings-County-Housing-Prediction-Model/blob/main/data/KC_Area.Final.jpg)

Home prices went down the further away they were from the downtown Seattle and Redmond areas.

![Image](https://github.com/grace-arina/Kings-County-Housing-Prediction-Model/blob/main/data/Home_Quality_Final.jpg)

Home prices rose as the quality of homes rose, leading us to believe that homesellers could get more bang for their buck by doing renovations.

Recommendations
---

Based on the above, we can recommend the following:

1. For homebuyers: Buy during the winter season and look into purchasing older homes as they tend to be less expensive the older they are.

2. For homesellers: Consider adding more bathrooms and fix up the house by improving quality of materials when buying and remodeling to sell at a higher price later on.

3. For those in the tech industry:  Look at homes outside of the downtown areas for more affordable homes

