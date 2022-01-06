# Kings-County-Housing-Prediction-Model

![Image](https://media.gettyimages.com/photos/sunset-seattle-picture-id615989790?k=20&m=615989790&s=612x612&w=0&h=Ai9z_Bp8yePIiFy6F5PO0KywqrYLfWW53VYSzL-2pW8=)

**Authors:** Grace Arina, Justin Sohn, Anthony Warren

##Business Problem
---

The goal is to save the new home buyers some time and to help ensure consistency in pricing between new houses on the market and old houses.

The main purpose of this algorithm is predictive, meaning that this model should be able to take in attributes of the King's County dataset that does not yet have a set price, and to predict a good price. The effectiveness of this predictive model will be measured by how well it predicts prices in our test set, where we know what the actual prices were but the model does not.

The secondary purpose of this algorithm is inferential, meaning that the model should be able to tell us something about the relationship between the attributes of a house in King's County and its price.

##Analysis Questions
---

This analysis will seek to answer three questions about the data:

**Question 1**: Which features are most highly correlated with price?

**Question 2**: Which features have the strongest correlations with other predictor variables?

**Question 3**: What combinations of features is the best fit, in terms of predictive power, for a multiple regression model to predict house prices?

##Data
---

We've used housing data from the King County dataset, which has records on houses sold from May 2014 to May 2015. 

##Methods
---

After cleaning the data for incorrect/missing values, we dropped the 'id' column as it wouldn't be useful going forward. Next, we've listed out the variables by type (categorical vs continuous) and plotted a corresponding heatmap for all of the non-dropped columns

![Image]Documents/Flatiron/phase_2/Kings-County-Housing-Prediction-Model/Correlation Heat Map.png

Next, we then perform a train-test split to train and eventually test a model to see how well it works with the newly obtained test data.

From here, we've obtained our baseline, numeric, and final models

##Results
---

##Recommendations
---

##Conclusion
---