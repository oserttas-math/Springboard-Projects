# Logistic Regression

Logistic regression models the probability that dependent variable Y bleongs to a particular category.The values of the probability ranges between 0 and 1. Based on the set threshold model makes the classification. Conventinally the threshold is accepted as 0.5. Logistic function is used in logistic regression $$ P(X) = \frac{\exp(\beta_0 + \beta_1*X}{1+ \exp(\beta_0 + \beta_1*X}.$$ and this yields $$ log(\frac{P(X)}{1-P(X)} = \beta_0 + \beta_1*X

The left-hand side is called the log-odds or logit. So to speak the logistic regression model has a logit that is linear in X.

---

# The Data

Each observation in the dataset of 10,000 includes the height and weight of either a male or female adult person.

---

# Description

This small project is a simple example of classifying the person gender based on the height and weight data to that person. Default class of the response variable `Gender` is male here so if the probability threshold was set to 0.5 than probabilities above 0.5 would return `male` person. 

In the project, we also discussed: 

- when `scaling` the data is needed and otherwise. 
- whether or not `regularization` helps getting more accurate model
- parameter tuning using the GridSearch method
- cross-validation using KFold method

---

# Notes
- Resources for scaling data can be reached [here](https://sebastianraschka.com/Articles/2014_about_feature_scaling.html) and [here](https://medium.com/greyatom/why-how-and-when-to-scale-your-features-4b30ab09db5e)
- Default example was taken from the text book Intro Statistical Learning.
- There is a problem when pipeline process applied to the data. It is to be solved. Any feedback would be appreciated. 
