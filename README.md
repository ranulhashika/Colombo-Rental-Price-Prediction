# Colombo House Rental Price Prediction Model 🏠📊

## Project Overview 🌍
This model predicts house rental prices in the Colombo district of Sri Lanka. It aims to provide accurate rental price predictions using machine learning techniques.

## Key Features ✨
- Predicts house rental prices based on various factors.
- Achieved an **R²** value of **0.79**.
- The dataset was scraped from publicly posted advertisements on Sri Lankan classified websites.

## Tech Stack 🛠️
- **Python**
- **Jupyter Notebook**
- **Pandas**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**
- **XGBoost**
- **NumPy**
- **Beautiful Soup**

## File Organization 📂
- `sl_rent_price_data.csv` (in the `data/` folder): The dataset used for training the model.
- `preprocessing.ipynb`: Preprocesses the dataset and saves it as `preprocessed_data.csv`.
- `training.ipynb`: Trains the model and exports the best-performing model as `model.pkl`.
- `predict.ipynb`: Uses the trained `model.pkl` to make predictions on new data. The `suburbs.csv` file is required for predictions.

## Usage Instructions ⚙️
1. Run the `predict.ipynb` notebook.
2. Ensure you have the `model.pkl` and `suburbs.csv` files in the same directory.
3. Follow the instructions in the notebook to make predictions.

## Data Sources 📥
- The data was scraped from publicly posted advertisements on Sri Lankan classified websites (from October 2024 onwards) using the BeautifulSoup library.
- The dataset includes the following columns:
  - **Advertisement posted date**
  - **No of bedrooms**
  - **No of bathrooms**
  - **House size**
  - **Land size**
  - **Suburb of Colombo**
  - **Monthly Rental**

## Model Description 🤖
- The model uses **Random Forest** regression, as it provided the best performance during training.

## Evaluation Metrics 📊
- The performance of the model is evaluated using the **R²** metric.
