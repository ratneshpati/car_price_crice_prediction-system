# car_price_crice_prediction-system
# Car Price Prediction

This repository contains a data science project focused on predicting car prices using machine learning techniques. The project demonstrates the full data science workflow, from raw data to a trained machine learning model. An interactive widget-based interface is also implemented for easy car price predictions.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Cleaning](#data-cleaning)
- [Modeling and Prediction](#modeling-and-prediction)
- [Interactive Widget Interface](#interactive-widget-interface)
- [Results and Evaluation](#results-and-evaluation)
- [Setup and Usage](#setup-and-usage)
- [Future Enhancements](#future-enhancements)

## Project Overview

The goal of this project is to predict the prices of used cars based on various attributes like make, model, year, kilometers driven, fuel type, and more. The steps involved include:

1. Importing and exploring the raw dataset.
2. Cleaning and preprocessing the data.
3. Building and training a machine learning model.
4. Evaluating the model’s performance.
5. Creating an interactive prediction interface using Jupyter widgets.

## Dataset

The dataset used in this project includes the following features:

- `Name`: Model of the car.
- `Company`: Manufacturer or brand of the car.
- `Year`: Manufacturing year.
- `Kms Driven`: Total kilometers the car has traveled.
- `Fuel Type`: Type of fuel used by the car.
- `Price`: Selling price of the car (target variable).

The raw data is available in the `data/` directory.

## Data Cleaning

Data cleaning is a crucial step in preparing the dataset for analysis and modeling. The following steps were performed:

- **Handling Missing Values**: Removed or imputed missing entries.
- **Data Transformation**: Converted non-numeric fields (e.g., `Company`, `Fuel Type`) to numeric values using one-hot encoding.
- **Feature Engineering**: Adjusted car names by extracting only the relevant words, and cleaned other features like `Kms Driven`.
- **Outlier Removal**: Identified and removed outliers to avoid skewing the model.

## Modeling and Prediction

The machine learning model is built using the scikit-learn library. The process includes:

1. **Model Selection**: Linear Regression is used as the primary model for price prediction.
2. **Training and Testing**: The dataset is split into training and testing sets for model evaluation.
3. **Hyperparameter Tuning**: Grid search or cross-validation can be used to fine-tune the model.
4. **Prediction**: The final model is used to predict car prices on new data based on user inputs.

## Interactive Widget Interface

An interactive interface has been implemented using Jupyter widgets, where users can input car details and get an estimated resale price for a car. The widgets used include dropdowns, sliders, and buttons for car attributes like:

- **Company**: Select the car brand.
- **Car Name**: Choose the car model based on the selected company.
- **Year**: Slider to input the manufacturing year.
- **Kms Driven**: Slider to input the number of kilometers driven.
- **Fuel Type**: Select the type of fuel (Petrol, Diesel, CNG, Electric).

The interface dynamically updates car models based on the selected company and displays the predicted price once the user fills in all details.

## Results and Evaluation

The model’s performance is evaluated using standard metrics:

- **Mean Absolute Error (MAE)**: Measures the average magnitude of errors in predictions.
- **Mean Squared Error (MSE)**: Emphasizes larger errors and helps in evaluating model accuracy.
- **R-squared Score**: Indicates how well the model explains the variance in the target variable.

### Results Visualization:
Plots and charts are used to visualize the model’s performance, comparing predicted values against actual prices.

## Setup and Usage

### Prerequisites

- Python 3.x
- Jupyter Notebook (optional but recommended)
- Required Python libraries: Pandas, NumPy, scikit-learn, Matplotlib, IPywidgets

### Installation Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/car-price-prediction.git
   cd car-price-prediction

