# airbnb-price-prediction
This project aims to identify variables impacting Airbnb rates in well-known European locations. By utilizing machine learning approaches, this project serves as a tool to predict Airbnb prices in various locations, aiding hosts in pricing their listings and providing insights for tourism stakeholders to understand local trends.

## Quarto Markdown (.qmd) File

The repository contains a Quarto Markdown (.qmd) file, which includes the code, analysis, and visualizations used in this project. Quarto is a versatile tool that allows for the creation of reproducible reports, combining code, markdown, and rich outputs in a single document. 

### How to Use the .qmd File

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
   - **Evaluation metrics** like RMSE to assess model performance.
   - **Discussion and insights** based on the results, with ethical considerations surrounding the use of these models in real-world applications.

## Usage

1. Load your dataset into the appropriate DataFrame variables: `training_df`, `val_df`, and `test_df`.
2. Run the code provided in the scripts to create training, validation, and test sets.
3. Fit the models and evaluate their performance using RMSE.

## Results

Results will be printed as RMSE values for training and validation sets for each model.

## Ethical Considerations

Stakeholders using this model should be aware of potential biases in the data, such as price discrimination among Airbnb listings, which could contribute to gentrification and housing shortages. To ensure fair application, the model should be reviewed by local stakeholders familiar with the area. This collaboration promotes equity and visibility across different interests, ensuring that decisions based on the model are informed and responsible.
