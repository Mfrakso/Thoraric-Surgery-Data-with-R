# Thoraric-Surgery-Data-with-R

This formula includes various preoperative health factors and the patient's age to predict the survival outcome.

Model Summary: The model's coefficients, standard errors, z-values, and p-values are displayed to assess the significance of each variable.

Model Evaluation:

The model's goodness-of-fit is evaluated using the Chi-Square Test for the deviance reduction.
The Chi-square value is calculated and the associated p-value is used to assess whether the model performs better than a random guess.
Odds Ratios: The odds ratios for each variable are calculated to interpret the impact of each feature on the survival prediction.

Model Performance
Null Model Log-Likelihood: 395.61
Fitted Model Log-Likelihood: 359.28
Model Chi-Square: 36.33 (p-value = 0.006)
Since the p-value is less than 0.05, we reject the null hypothesis and conclude that the model is significantly better than random chance at predicting the survival outcome.

Variables with Greatest Effect
The variables with the greatest impact on survival prediction (in order of importance) are:

PRE17: Type 2 Diabetes Mellitus
PRE30: Smoking status
PRE7: Pain before surgery
AGE: Age at surgery
PRE11: Weakness before surgery
These variables have the most significant effects on the predicted outcome.

How to Use
Clone this repository.
Load the data into R using the provided script.
Run the Logistic Regression model to predict survival probability based on patient data.
Use the summary() and exp() functions to interpret the model coefficients and odds ratios.
Dependencies
R (version 4.0 or higher)
foreign package (for reading ARFF files)
glm() function (for fitting the logistic regression model)
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
This dataset is commonly used in survival analysis and machine learning tutorials. The methodology used here demonstrates how logistic regression can be applied to medical datasets for predictive modeling.
