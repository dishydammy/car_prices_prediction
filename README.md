# Car Prices Prediction 🚗📊
This repository contains the code and resources for a data science project on car price prediction. This project was developed as a hackathon submission for qualification for the Data Science Nigeria (DSN) AI Bootcamp 2025.

The goal of this project is to build a machine learning model that accurately predicts the prices of cars based on various features.


## ⚙️ Project Structure
The project is organized into the following directories and files:

- `requirements.txt`: A list of all necessary Python libraries and their versions.
- `car_prices_prediction_notebook/`: The notebooks for Exploratory Data Analysis (EDA), where I explored the dataset, visualized key relationships, and handled data cleaning and preprocessing and where the machine learning models were trained, evaluated, and the final model was selected.


## 🔍 Data
The dataset used for this project was provided as part of the DSN AI Bootcamp 2025 hackathon. It includes a variety of features that influence a car's price. The key features used in this project are:

- **Brand & Model**: The manufacturer and specific model of the car.
- **Model Year**: The year the car was manufactured.
- **Milage**: The total distance the car has traveled.
- **Fuel Type**: The type of fuel the car uses (e.g., gasoline, diesel, electric).
- **Engine Type**: Engine specifications.
- **Transmission**: The type of transmission (e.g., automatic, manual).
- **Exterior & Interior Colors**: The color of the car's exterior and interior.
- **Accident History**: A history of any prior accidents or damage.
- **Clean Title**: The status of the vehicle's title.
- **Price**: The target variable to be predicted.


## 🧠 Methodology
The problem was framed as a regression task, aiming to predict a continuous numerical value (the car's price). I explored and compared three different gradient boosting models to find the best-performing one.

- CatBoost
- LightGBM
- XGBoost

I utilized Optuna to perform hyperparameter finetuning to get the best performance out of the models.

After extensive training and evaluation, the CatBoost model was chosen as the final model due to its superior performance on the validation set.

✅ Results
The best-performing model, CatBoost, achieved a Root Mean Squared Error (RMSE) of 72697.


## 🚀 Getting Started
Follow these instructions to set up the project locally and reproduce the results.

**Prerequisites**
- Python 3.8+
- pip

**Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/dishydammy/car_prices_prediction.git
   cd car_prices_prediction
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

**Running the Notebooks**
1. Launch Jupyter Notebook or JupyterLab:
   ```bash
   jupyter notebook
   ```
2. Run the model training and evaluation notebook "car_prices_prediction_notebook".
