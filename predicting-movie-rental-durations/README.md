# DVD Rental Duration Prediction

This project aims to predict the number of days a customer rents DVDs for using regression models.

## Project Overview

The analysis involves preprocessing rental data, creating relevant features, and developing a regression model to predict rental duration. The goal is to achieve a mean squared error (MSE) of less than 3 on the test set.

## Data Source

The project uses a dataset named `rental_info.csv` containing information about DVD rentals.

## Project Objectives

1. Preprocess the rental data.
2. Create relevant features for prediction.
3. Develop and evaluate regression models.
4. Recommend the best performing model.

## Key Outputs

- `X`: DataFrame containing features for regression.
- `y`: Series containing the target variable (rental duration).
- `best_model`: The recommended regression model.
- `best_mse`: Mean Squared Error of the best model on the test set.

## Getting Started

### Prerequisites

- Python enviroment
- pandas
- scikit-learn

Or just use Google colab for ease of use

## Methodology

1. **Data Loading and Preprocessing**: 
   - Load the `rental_info.csv` file using pandas.
   - Create a `rental_length_days` column from `return_date` and `rental_date`.
   - Generate dummy variables for specific `special_features`:
     - `deleted_scenes`: 1 if "Deleted Scenes" is present, 0 otherwise.
     - `behind_the_scenes`: 1 if "Behind the Scenes" is present, 0 otherwise.

2. **Feature Selection**:
   - Create DataFrame `X` with appropriate features.
   - Select `rental_length_days` as the target variable (`y`).

3. **Data Splitting**:
   - Split data into training (80%) and test (20%) sets.
   - Use `random_state=314` for reproducibility.

4. **Model Development and Evaluation**:
   - Implement LASSO and Random Forest.
   - Evaluate models using Mean Squared Error (MSE) on the test set.
   - Select the best performing model (MSE < 3).

5. **Result Storage**:
   - Save the best model as `best_model`.
   - Store the MSE of the best model as `best_mse`.

## Potential Modeling Approaches

- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regression
- Gradient Boosting Regression

## Feature Engineering Considerations

- Encoding categorical variables (if any)
- Handling missing values (if present)
- Normalizing or standardizing numerical features
- Creating interaction terms between features

## Evaluation Metric

- Mean Squared Error (MSE): The average squared difference between the predicted and actual rental durations.
- Goal: Achieve MSE < 3 on the test set.

## Limitations and Considerations

- The analysis assumes that past rental behavior is indicative of future behavior.
- External factors affecting rental duration (e.g., holidays, promotions) may not be captured in the dataset.

## Potential Extensions

- Implement cross-validation for more robust model evaluation.
- Explore feature importance to understand key drivers of rental duration.
- Develop an ensemble model combining multiple regression techniques.
- Analyze residuals to identify potential areas for model improvement.

## Results Interpretation

- The `best_model` represents the regression model that provides the most accurate predictions of rental duration.
- `best_mse` indicates the average squared prediction error in days. A lower MSE suggests better model performance.