# supervised_machine_learning

# Intro

The purpose of this project was to use introduce some concept of Supervised Learning in Machine Learning Models.
The two models being used are:
- Random Forest
&
- Logistic Regression

# Data Set 

![Train Data](2019loans.csv)
![Test Data](2020Q1loans)

The data set was a collection of user bank/credit information that will be evaluated using the above machine learning models to gauge which accounts are either high or low risk for a loan.

# Method

The data is loaded in, processed by turning all Text information into binary information for use in the machine learning models later. We then scan each dataframe to verify that each has the same number of columns and if not, the missing column(s) will be added and set to 0 as there would be no information within them. This preserves the formatting between the datasets to ensure limited information loss.

Afterwards the data is separated into Test and Train sets, fit to two separate models and the results are evaluated.

Once complete we are able to observe the results but this instance is completed with data that is not scaled, meaning that columns within the data set that have largely differing ranges will have separate impacts on the result from the Models.
> e.g. a column ranging from 1-100 will have a smaller impact than one ranging from 1-1,000,000.

This will not due for the creation of an accurate model, with exception to the Random Forest Model, so we move to scaling the data and re-training the models to display the overall change in accuracy after the impact of each feature within the data has been normalized.

> Exception Explanation: Random Forests Models don't take into account the relationship between each predictor variable and the response so scaling the data before running usually produces better results.


# Analysis

## Results:

### Logistic Regression:
- Unscaled Data: 52.6%
- Min Max Scaler: 59.5% 
- Standard Scaler: 66.1%
### Random Forest Model:
- Unscaled Data: 61.7%
- Min Max Scaler: 61.8%
- Standard Scaler: 61.7%

-------------------------------------------------------------------------------------------------------------------------------------

One of the aspects of machine learning is testing models and data to conclude which combination works best without over fitting the data and producing a useless model. When comparing the scores between types of scaled data, the Standard Scaler produced better results with the Logistic Regression Model improving by 11% after scaling. Moving from a model that flips a coin to a model that makes an educated yet uncertain guess.

When running the unscaled data the results for the Random Forest Model were better with the unscaled data but not significantly, 0.1%, meaning that this data simply doesn't fit a random forest model.

# Conclusion

In this project we observed a seemingly useful Logistic Regression Model using Standard Scaled data and a Random Forest Model that perform equally with both types of data (scaled & unscaled). The next step toward creating an improved model would be Cross Validating parameters and evaluating resulting scores, implementing Feature Reduction, testing different models, or even changing perspective and asking a different question after considering the story of the data.


