Abalone Age Prediction Using Generalized Additive Models

# Overview

This project uses a **Generalized Additive Model (GAM)** to predict abalone age (Rings) from physical measurements in the Kaggle Abalone Dataset. GAMs were chosen because they can model non-linear relationships while remaining interpretable.

# Dataset

**Target Variable:** Rings

**Features:**
- Sex
- Length
- Diameter
- Height
- Whole Weight
- Shucked Weight
- Viscera Weight
- Shell Weight

# Feature Engineering

The following features were created:

- Shell Ratio
- Length-to-Diameter Ratio
- Volume
- Density

These variables help capture biological growth characteristics.

# Data Preparation

- Encoded categorical variables
- Applied log transformation to the target variable
- Split data into training and validation sets (80/20)

# Model

A **Generalized Additive Model (GAM)** was built using the `pyGAM` library with spline functions for continuous variables and a factor term for sex.

# Results

| Model | RMSLE |
|---------|---------|
| GAM | **0.1564** |

The GAM successfully captured non-linear relationships and achieved strong predictive performance.

# Visualizations

The project includes:

- Actual vs. Predicted Plot
- Residual Plot
- Partial Dependence Plots

These visualizations help evaluate model performance and interpret predictor effects.

# Key Findings

- Non-linear relationships exist within the dataset.
- Feature engineering improved model performance.
- GAM provided accurate and interpretable predictions.

# Technologies

- Python
- Pandas
- NumPy
- Scikit-Learn
- pyGAM
- Matplotlib

