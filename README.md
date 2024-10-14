# About The Project
This project aims to identify variables impacting Airbnb rates in well-known European locations. By utilizing machine learning approaches, this project serves as a tool to predict Airbnb prices in various locations, aiding hosts in pricing their listings and providing insights for tourism stakeholders to understand local trends. The models compared include:

* Multiple Linear Regression
* Ridge Regression
* Random Forest

## Motivation  

Travel has significantly increased post-pandemic, leading to a surge in demand for vacation accommodations. Airbnb is widely used by travelers to find flexible lodging options. Understanding the factors that impact Airbnb prices is critical for both hosts and tourism stakeholders, helping them make informed decisions about pricing and market trends.This project aims to identify variables impacting Airbnb rates in well-known European locations. By utilizing machine learning approaches, this project serves as a tool to predict Airbnb prices in various locations, aiding hosts in pricing their listings and providing insights for tourism stakeholders to understand local trends. The models compared include:

### Built With

- **Python**
- **R** (via `reticulate` in Quarto)
- **Quarto**: Used to create the `.qmd` file and render the analysis report.
- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations.
- **Seaborn**: For data visualization.
- **Scikit-learn**: For machine learning models (Multiple Linear Regression, Ridge Regression, and Random Forest) and evaluation metrics.
- **GridSearchCV**: For hyperparameter tuning to optimize model performance.
  

### Data

The dataset used for this project is located in the `data` folder:

* `airbnb_prices.csv`: Contains Airbnb listing information such as room type, host information, location, and listing price.





## Getting started  
### Quarto Markdown (.qmd) File

The repository contains a Quarto Markdown (.qmd) file, which includes the code, analysis, and visualizations used in this project. You can view the fully rendered file as a .pdf in the `results` folder. 

#### How to Use the .qmd File

1. **Viewing the .qmd file**: You can view the file directly in the repository, where the markdown content will render, but the code execution outputs may not display unless you render the document locally.

2. **Rendering the .qmd file**: 
   - To render the `.qmd` file on your local machine, make sure you have Quarto installed. You can follow the installation instructions from the [Quarto website](https://quarto.org/docs/get-started/).
   - Once Quarto is installed, open the terminal or command line and navigate to the repository folder.
   - Run the following command to render the document:
     ```bash
     quarto render airbnb_prices.qmd
     ```
   - This will produce a fully rendered HTML or PDF document with both the markdown explanations and code outputs.

3. **Exploring the Code and Analysis**: The `.qmd` file contains:
   - **Data preprocessing steps** such as scaling and splitting datasets.
   - **Machine learning models** (Multiple Linear Regression, Ridge Regression, Random Forest) used to predict Airbnb prices.
   - **Evaluation metrics** like RMSE amd data visualizations to assess model performance.
   - **Discussion and insights** based on the results, with ethical considerations surrounding the use of these models in real-world applications.

## Usage

1. Load your dataset into the appropriate DataFrame variables: `training_df`, `val_df`, and `test_df`.
2. Run the code provided in the scripts to create training, validation, and test sets.
3. Fit the models and evaluate their performance using RMSE.

## Results

Results will be printed as RMSE values for training and validation sets for each model.



