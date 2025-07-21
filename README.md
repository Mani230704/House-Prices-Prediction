# 🏡 Bangalore House Price Prediction

This project aims to predict the prices of residential properties in Bangalore using machine learning. It involves an end-to-end pipeline — from data preprocessing and model building to deploying a web-based application using Flask.

---

## 📌 Project Objective

To develop a machine learning model that predicts house prices in Bangalore based on features such as location, size (BHK), square footage, and number of bathrooms. The goal is to assist users in estimating property values and making informed real estate decisions.

---

## 📊 Dataset Description

- **Source**: Kaggle or curated dataset of Bangalore property listings
- **Target Variable**: `price` (in Lakhs)
- **Key Features**:
  - `location` – Area/Locality in Bangalore
  - `total_sqft` – Total built-up area in square feet
  - `bath` – Number of bathrooms
  - `bhk` – Number of bedrooms/hall/kitchen

---

## 🛠️ Technologies Used

- **Languages**: Python
- **Libraries**:
  - Data Handling: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  - Modeling: `scikit-learn`
- **Framework**: Flask (for deployment)
- **Tools**: Jupyter Notebook, VS Code

---

## 📂 Project Structure

bangalore-house-price-prediction/
│
├── data/ # Raw and cleaned dataset files
├── model/ # Trained model saved as .pkl
├── notebooks/
│ └── Bangalore_House_Price_Prediction.ipynb # Jupyter notebook with EDA + modeling
├── app/
│ ├── templates/
│ │ └── index.html # Frontend HTML template
│ └── app.py # Flask app script
├── requirements.txt # List of Python dependencies
└── README.md # Project documentation


---

## 🔍 Exploratory Data Analysis (EDA)

- Handled missing and inconsistent values
- Standardized unit conversions (e.g., sqft ranges)
- Removed outliers in sqft per BHK
- Used `location` dimensionality reduction to handle rare categories

---

## 🤖 Model Development

- **Algorithm Used**: Linear Regression
- **Preprocessing**:
  - Converted categorical variables using One-Hot Encoding
  - Removed multicollinearity
- **Model Evaluation**:
  - R² Score
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)

---

## 🧪 Example Model Metrics

- **R² Score**: ~0.82
- **MAE**: ~5.3 Lakhs
- **RMSE**: ~7.1 Lakhs

> *Note: Metrics may vary slightly based on dataset and preprocessing.*

---

## 💻 Web Application (Flask)

An interactive web interface built with Flask that takes user input such as location, BHK, sqft, and number of bathrooms and returns a predicted price.

### Run Locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/bangalore-house-price-prediction.git
   cd bangalore-house-price-prediction
   
2.Install dependencies:

   ```bash
   pip install -r requirements.txt
   Start the Flask application:streamlit run 

3.Run the Application
   ```bash
   cd app
   python app.py
   Open your browser and go to: http://127.0.0.1:5000


