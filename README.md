# Restaurant Revenue Prediction using Decision Tree Regression

This Jupyter Notebook contains Python code for predicting restaurant revenue using a Decision Tree Regression model. The model utilizes various features related to restaurants to predict their revenue.

## Dataset Columns

- **Name**: The name of the restaurant.
- **Location**: The geographical location of the restaurant (e.g., city or region).
- **Cuisine**: The type of cuisine served at the restaurant.
- **Rating**: The rating of the restaurant based on customer reviews.
- **Seating Capacity**: The number of seats available in the restaurant.
- **Average Meal Price**: The average price of a meal at the restaurant.
- **Marketing Budget**: The budget allocated for marketing activities.
- **Social Media Followers**: Number of followers on social media platforms.
- **Chef Experience Years**: Years of experience of the head chef.
- **Number of Reviews**: Total number of customer reviews received.
- **Avg Review Length**: Average length of customer reviews.
- **Ambience Score**: Score rating the ambience of the restaurant.
- **Service Quality Score**: Score rating the quality of service at the restaurant.
- **Parking Availability**: Whether parking is available at the restaurant (Yes/No).
- **Weekend Reservations**: Number of reservations made for weekends.
- **Weekday Reservations**: Number of reservations made for weekdays.
- **Revenue**: Actual revenue generated by the restaurant (target variable for prediction).

## Prerequisites

- Jupyter Notebook (or JupyterLab) installed
- Python 3.x
- Libraries:
  - pandas
  - scikit-learn (sklearn)
  - matplotlib

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/ChaitanyaParate/Restaurant-Revenue-Prediction.git
   cd Restaurant-Revenue-Prediction
2. Install the required libraries:

   pip install pandas scikit-learn matplotlib

##Usage

1. Open the Jupyter Notebook:
    jupyter notebook decision_tree_regression.ipynb
   
3. Execute the cells in the notebook sequentially to run the code.
  
4. Ensure the dataset restaurant_data.csv is present in the same directory as the notebook or modify the file path in the code accordingly.
  
6. View the results including average R-squared score and the plotted decision tree.

## Code Explanation
The Jupyter Notebook contains the following sections:

### Data Preprocessing:

1. Reads the restaurant data from restaurant_data.csv.
2. Encodes categorical variables (Location and Cuisine) using one-hot encoding (pd.get_dummies).
3. Converts Parking Availability into binary values (1 for 'Yes' and 0 for 'No').
### Model Training:

1. Splits the data into training and testing sets using train_test_split.
2. Initializes a Decision Tree Regressor with a specified max_depth and random_state.
3. Performs 10-fold cross-validation to evaluate the model's performance using r2_score.
### Visualization:

Plots the trained Decision Tree using tree.plot_tree from sklearn.

## Parameters
max_depth: Controls the maximum depth of the Decision Tree.
test_size: Determines the proportion of the dataset to include in the test split.
## Results
The notebook computes the average R-squared score across 10 folds of cross-validation, providing an evaluation of the model's predictive performance.
