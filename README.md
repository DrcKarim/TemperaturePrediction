# TemperaturePrediction
Weather Prediction Model

Overview

This project builds a weather prediction model to estimate temperature based on input features such as humidity, wind speed, pressure, and cloud cover. Multiple regression models are trained and evaluated to determine the best-performing one.

Features Used

Humidity (%)

Wind Speed (km/h)

Pressure (hPa)

Cloud Cover (%)

Temperature (°C) (Target Variable)

Steps in the Model Development

1. Import Libraries

To handle data, perform calculations, and build machine learning models, the following libraries are used:

pandas – For data manipulation.

numpy – For numerical computations.

scikit-learn – For machine learning tasks such as model training, scaling, and evaluation.

2. Load and Prepare Data

Read the dataset from a CSV file.

Remove unnecessary columns.

Define input features and the target variable (temperature).

3. Split Data

Divide the dataset into two subsets:

Training set (80%) – Used to train the model.

Testing set (20%) – Used to evaluate the model’s performance.

4. Standardize Features

Normalize input features to ensure they are on a similar scale (zero mean, unit variance).

Standardization improves model performance and training efficiency.

5. Initialize Models

Create multiple regression models to compare their performance, including:

Linear Regression

Lasso Regression

Ridge Regression

ElasticNet Regression

SGD Regressor

6. Train Models

Train each model using the training data to learn the relationship between input features and temperature.

7. Predict and Evaluate

Use the trained models to make predictions.

Evaluate each model using key performance metrics:

Mean Squared Error (MSE) – Measures the average prediction error (lower is better).

R² Score – Represents model accuracy as a percentage (higher is better).

8. Display Results

Print the error and accuracy of each model to compare their effectiveness.

9. User Input for Prediction

Allow users to enter values for humidity, wind speed, pressure, and cloud cover.

Standardize the input to match the trained model’s scale.

Use one of the trained models (e.g., Linear Regression) to predict the temperature based on the user's input.

Display the predicted temperature.

How to Use

Run the script to train the models.

Enter climate conditions as prompted.

Receive the predicted temperature as output.

Dependencies

Make sure you have the following Python libraries installed:

pip install pandas numpy scikit-learn matplotlib

Future Improvements

Add more weather-related features for better accuracy.

Implement deep learning models for prediction.

Deploy the model as a web application.
