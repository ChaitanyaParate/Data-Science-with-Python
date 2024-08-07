# Automobile Mileage Prediction

This repository contains a Python script for predicting automobile mileage using various regression models. The script performs data preprocessing, model training, and evaluation using several machine learning algorithms. 

## Features

- Data preprocessing with K-Nearest Neighbors imputation for missing values.
- Scaling of features using `StandardScaler`.
- Comparison of multiple regression models, including:
  - Random Forest Regressor
  - Decision Tree Regressor
  - Bagging Regressor
  - Linear Regression
- Model evaluation using metrics like R² score and Mean Squared Error (MSE).
- Visualization of residuals vs. fitted values.

## Files

- `Automobile.csv`: The dataset used for training and testing the models.
- `predictive_modeling.py`: The main script containing data preprocessing, model training, and evaluation.

## Requirements

To run this script, you need the following Python packages:
- pandas
- scikit-learn
- matplotlib

You can install the required packages using `pip`:

pip install pandas scikit-learn matplotlib

## Usage

1. **Download the dataset**: Ensure you have the `Automobile.csv` file in the same directory as the script.

2. **Run the script**: Execute the script using Python:

    python predictive_modeling.py

3. **Output**:
   - The script prints the best parameters for the Random Forest model based on MSE and R² score.
   - It also displays the average R² score for the Decision Tree model using 10-fold cross-validation.
   - Finally, it prints R² scores for the Bagging Regressor and Linear Regression models.

4. **Visualization**:
   - The script generates a scatter plot of residuals vs. fitted values for the Random Forest model.

## Code Explanation

- **Data Preprocessing**:
  - Missing values in the dataset are imputed using K-Nearest Neighbors.
  - Features are scaled using `StandardScaler`.

- **Model Training and Evaluation**:
  - Several regression models are trained and evaluated.
  - For the Random Forest model, different values of `max_leaf_nodes` are tested to find the best configuration.
  - The Decision Tree model is evaluated using 10-fold cross-validation.
  - Bagging Regressor and Linear Regression models are trained and their performance is evaluated.

- **Visualization**:
  - A scatter plot of residuals vs. fitted values for the Random Forest model is created to assess the model's performance visually.

## Contributing

Feel free to fork the repository and submit pull requests. If you find any issues or have suggestions for improvements, please open an issue or contact the repository maintainer.

## Acknowledgments

- The `Automobile.csv` dataset is used for educational purposes.
- The implementation uses `scikit-learn` for machine learning models and `matplotlib` for visualization.
