# Heart Disease Prediction Model

This project aims to predict the likelihood of heart disease based on various medical attributes using machine learning techniques.

## Dataset

The dataset used in this project is stored in the `heart.csv` file. It contains the following columns:

- `age`: Age of the patient
- `sex`: Gender (0 = female, 1 = male)
- `cp`: Chest pain type (0 = typical angina, 1 = atypical angina, 2 = non-anginal pain, 3 = asymptomatic)
- `trestbps`: Resting blood pressure (in mm Hg)
- `chol`: Serum cholesterol (in mg/dl)
- `fbs`: Fasting blood sugar > 120 mg/dl (0 = false, 1 = true)
- `restecg`: Resting electrocardiographic results (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy)
- `thalach`: Maximum heart rate achieved
- `exang`: Exercise induced angina (0 = no, 1 = yes)
- `oldpeak`: ST depression induced by exercise relative to rest
- `slope`: Slope of the peak exercise ST segment (0 = upsloping, 1 = flat, 2 = downsloping)
- `ca`: Number of major vessels (0-3) colored by fluoroscopy
- `thal`: Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect)
- `target`: Presence of heart disease (0 = no, 1 = yes)

## Model Training

The dataset is split into training and testing sets using the `train_test_split` function from the `sklearn.model_selection` module. The features (`x`) are standardized using `StandardScaler` to ensure that each feature contributes equally to the model. Polynomial features of degree 3 are created using `PolynomialFeatures` to capture nonlinear relationships. The model is trained using a linear regression algorithm from `sklearn.linear_model` package.

## Evaluation

The model's performance is evaluated using the R² score, which measures the proportion of the variance in the dependent variable that is predictable from the independent variables. The R² score ranges from 0 to 1, where a higher value indicates a better fit of the model to the data.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn

## Instructions

1. Install the required dependencies using pip:

2. Place the `heart.csv` file containing the dataset in the same directory as the Python script.

3. Run the Python script to train the model and evaluate its performance.

## Author

[Chaitanya Parate]

