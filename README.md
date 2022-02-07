# supervised_machine_learning


# Web-Design-Challenge

# Intro

The purpose of this project was to use introduce some concept of Supervised Learning in Machine Learning Models.
The two models being used are:
- Random Forest
&
- Logistic Regresson

# Data Set 

![Train Data](2019loans.csv)
![Test Data](2020Q1loans)


The data set was a collection of user bank/credit information that will be evaluated using the above machine learning models to guage which accounts are either high or low risk for a loan.

# Method

The data is loaded in, processed by turning all Text information into binary information for use in the machine learning models later. We then scan each dataframe to verify that each has the same number of columns and if not, the missing column(s) will be added and set to 0 as there would be no information within them. This preserves the formatting between the datasets to ensure limited information loss.

Afterwards the data is separated into Test and Train sets, fit to two separate models and the results are evaluated.

Once complete we are able to observe the results but this instance is completed with data that is not scaled, meaning that columns within the data set that have largely differing ranges will have separate impacts on the result from the Models.
> e.g. a column ranging from 1-100 will have a smaller impact than one ranging from 1-1,000,000.

This will not due for the creation of an accurate model, with exeption to the Random Forest Model, so we move to scaling the data and re-training the models to display the overall change in accuracy after the impact of each feature within the data has been normalized.

> Exception Explanation: Random Forests Models don't take into account the relationship betwee each predictor variable and the response so scaling the data before running usually produces better results.



# Analysis
When running the unscaled data the results for 


# Conclusion

Using HTML and CSS to display information is a major component of the age we live in. anytime someone searches for information or even used the web they're looking at a programs interpretation of styles and code to transfer information. After completing this assignment, I don't think that I'll be able to see a web page without think about the code and styles used to make the page appear as it does.

Making sure that the aspects needed in each page were behaving as desired or pinpointing the part of the code I wanted to style using CSS was a challenge due mostly to my novice-level experience in this coding language. I enjoyed overcoming obstacles that were almost certainly constructed by myself and also by accident. The relief of getting something to work after fiddling with it for an hour was a confusing mix of accomplishment and shame.

In the end, once I had all seven pages set up with links to each and feature such as click-able photos that take one to the corresponding web page and a pop-out button on the Nav-bar, it felt pretty nice to have tackled what at this point in time is a big concept but in retrospect will probably be the equivalent to a "Hello World!" statement.


