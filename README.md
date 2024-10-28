# Biking Rental Predictor

> This project builds a multiple linear regression (MLR) model to predict bike rentals based on various factors, such as weather conditions, season, and holidays. The model aims to provide accurate predictions without overfitting or underfitting.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## General Information
- **Background**: This project was inspired by a passion for learning Artificial Intelligence and implementing MLR as an introductory model. The goal was to create a model that performs well without overfitting.
- **Problem Statement**: The objective is to predict bike rental counts (`cnt`) based on factors such as temperature, humidity, windspeed, season, and holiday status. Understanding these relationships helps in forecasting demand for bike rentals, aiding in resource allocation for bike-sharing services.
- **Dataset**: The dataset was provided by upGrad, split into 70-30 for training and testing, respectively. It contains features like weather conditions, date-related variables, and daily bike rental counts.

## Conclusions
- **Model Performance**: The model achieved an **R-squared of 0.821** on training data, explaining over 82% of the variance in bike rental counts.
- **Significant Predictors**:
  - **Year (`yr`)**: Strong predictor; rentals increased in 2019 compared to 2018.
  - **Temperature (`temp`)**: Positive impact on rentals, indicating more people rent bikes on warmer days.
  - **Holiday (`holiday`)**: Negative effect, suggesting fewer rentals on holidays.
  - **Humidity (`hum`)** and **Windspeed (`windspeed`)**: Both negatively impact rentals, as adverse weather conditions reduce demand.
  - **Seasonal Dummies**: Winter and spring show significant variations in rentals compared to the base season (fall).
- **Multicollinearity**: Initial analysis showed high multicollinearity between `temp` and `atemp`, which was resolved by removing `atemp` (Variance Inflation Factor (VIF) = 51.86).

## Technologies Used
- `pandas` - 1.3.3
- `numpy` - 1.21.2
- `scikit-learn` - 0.24.2
- `statsmodels` - 0.12.2
- `seaborn` - 0.11.2
- `matplotlib` - 3.4.3

## Acknowledgements
- This project was inspired by the upGrad coursework and assignments.
- Special thanks to mentors and instructors for guidance on MLR and data preprocessing techniques.

## Contact
Created by [@your-github-username] - feel free to reach out!

