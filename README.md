# Data Generation using Modelling and Simulation for Machine Learning

### Overview

In many real-world scenarios, collecting large datasets is difficult, expensive, or time-consuming. In such situations, modelling and simulation can be used to generate synthetic data that mimics real-world behavior.

In this project, I created a simple plant growth simulation model to generate synthetic data. This generated data was then used to train and compare different machine learning models.

The main goal of this assignment was to understand:

How simulation can generate structured datasets

How to run multiple simulations with random parameters

How to train ML models on synthetic data

How to compare models using evaluation metrics


# Problem Statement

We simulate plant growth based on three input factors:
Sunlight (hours per day)
Water (liters per day)
Fertilizer (units)

The output of the simulation is:
Final plant height

The objective is to train machine learning models to predict plant height based on the given inputs.

# Simulation Model

The plant growth is calculated using a simple mathematical formula:

Plant Height = 2 × Sunlight + 1.5 × Water + 3 × Fertilizer + Random Noise

Random noise is added to simulate natural variation, since real-world systems are never perfectly deterministic.

# Data Generation Process

Random values were generated within the defined parameter bounds.

These values were passed into the simulation function.

The final plant height was recorded.

This process was repeated multiple times.

A dataset of 1000 simulated samples was generated.

Final Dataset Columns:

sunlight

water

fertilizer

plant_height (target variable)


# Machine Learning Models Used

The following models were trained and evaluated:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

K-Nearest Neighbors

# Evaluation Metrics

The models were evaluated using:

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R² Score

The R² score was mainly used to compare model performance.

# Results

Since the simulation follows a mostly linear relationship, Linear Regression performed well.

Tree-based models such as Random Forest also showed strong performance because they can handle non-linear variations introduced by noise.

The best-performing model was selected based on the highest R² score and lowest error metrics.


# Conclusion

This project demonstrates how modelling and simulation can be used to generate meaningful datasets for machine learning tasks.

The approach can be extended to more complex systems such as:

Traffic flow prediction

Resource allocation

Supply chain modelling

Environmental systems

This assignment helped strengthen my understanding of both simulation techniques and machine learning model evaluation.

## AUTHOR - KANISHKA RANI (102317165)



