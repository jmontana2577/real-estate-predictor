# Real Estate Predictor
This project was assigned as part of the <a href="https://generalassemb.ly/education/data-science-immersive">Data Science Immersive</a> course at General Assembly.  

## Business Case

You work for a real estate company interested in using data science to determine the best properties to buy and re-sell. Specifically, your company would like to identify the characteristics of residential houses that estimate the sale price and the cost-effectiveness of doing renovations for resale.

The assigned project had three components, but I am only currently addressing the first two:

1. Estimate the sale price of properties based on their "fixed" characteristics, such as neighborhood, lot size, number of stories, etc.
1. Estimate the value of possible changes and renovations to properties from the variation in sale price not explained by the fixed characteristics. The goal is to estimate the potential return on investment (and how much one should be willing to pay contractors) when making specific improvements to properties.

---

## The Data
This project uses the [Ames housing data recently made available on kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques).

The original dataset contains 1385 properites from Ames, IA and there are 81 property features.

---

## The Process

Though the housing data for this project is very rich, it is not trivial to clean and prepare for modeling. Good EDA, cleaning, and feature engineering will be critical to the success of your models. Always remember to think critically about the data before modeling. The computer can't be the researcher for you!

The first two parts of the project are regression problems. There are potentially hundreds of features and plenty of multicollinearity, so regularization is definitely recommended.

The second question involves fitting a regression on the residuals of the first model. This is a practice that "covaries out" any effects of the predictors in the first model before investigating the effects of predictors in the second model.

The third section of the project is more challenging and involves dealing with significant class imbalance. This is a common and tricky problem in real-world classification tasks. We leave it up to you to decide how you want to tackle this problem and devise a solution, and highly recommend doing your own research into the topic.

We will be looking for the following things:

- Detailed EDA with justification for the steps. Visualize your data with pandas, matplotlib, or other plotting libraries. Explain the variables you choose for your models.
- Detail your choice of regression and classification models for the task. Include Markdown explaining your justification, results, and interpretation of your models. Make sure your code is clean and clear.
- Remember to frame your results according to your goals outlined in the project prompts.

---

## The Results

```
- Materials must be in a clearly commented Jupyter notebook
- You should demonstrate the ability to:

    - Analyze a complex dataset & explicitly state your assumptions.
    - Clean, impute, and explore the dataset.
    - Justify your modeling choices and feature engineering.
    - Plot, visualize, and interpret your data logically.
    - Clearly outline your modeling strategy in response to the questions
    - Explain your results to a technical audience.
```
---

## Next Steps

1. Split the data into training and test ses differently (randomly instead of based on year built), retrain the model and compare results.
1. Explore the possibility of more specific and robust recommendations for which features to renovate and how much to spend for each.
1. Revisit the classifiation aspect of this project (not currently addressed here) in which the goal is to identify abnormal sales. 
