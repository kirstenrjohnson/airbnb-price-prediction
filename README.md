# airbnb-price-prediction
This project aims to identify variables impacting Airbnb rates in well-known European locations. By utilizing machine learning approaches, this project serves as a tool to predict Airbnb prices in various locations, aiding hosts in pricing their listings and providing insights for tourism stakeholders to understand local trends.

## Usage

1. Load your dataset into the appropriate DataFrame variables: `training_df`, `val_df`, and `test_df`.
2. Run the code provided in the scripts to create training, validation, and test sets.
3. Fit the models and evaluate their performance using RMSE.

## Results

Results will be printed as RMSE values for training and validation sets for each model.

## Discussion of Results

This project compared three models for predicting airbnb prices: Multiple Linear Regression (MLR), Ridge Regression, and Random Forest.

* **Multiple Linear Regression** exhibited high bias and underfitting, performing the worst in terms of RMSE on both training and validation sets. The absence of interaction terms and polynomial features limited its complexity and predictive power, resulting in a less effective model.
* **Ridge Regression** showed slightly better performance than MLR, as it incorporates an alpha term that adds complexity and reduces variance. However, it still underfit the data compared to the Random Forest model. The scatter plots for MLR and Ridge were nearly identical.
* **Random Forest** achieved the lowest RMSE on the validation set, capturing complex, non-linear relationships between variables. While it has higher variance, the number of trees helps manage the bias-variance trade-off. Grid search for hyperparameter tuning selected 50 trees as the optimal parameter, though the increased complexity of the model reduces interpretability compared to MLR and Ridge.

## Ethical Considerations

Stakeholders using this model should be aware of potential biases in the data, such as price discrimination among Airbnb listings, which could contribute to gentrification and housing shortages. To ensure fair application, the model should be reviewed by local stakeholders familiar with the area. This collaboration promotes equity and visibility across different interests, ensuring that decisions based on the model are informed and responsible.
