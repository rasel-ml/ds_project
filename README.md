# Weather Prediction and Analysis Web App

## Overview
This project is a Django-based web application that allows users to:
- **Predict weather conditions** (rainfall or temperature) based on historical data.
- **Visualize weather trends** using uploaded datasets.
- **Analyze weather patterns** using machine learning techniques.
- **Update weather-related datasets.**

The project was developed as part of the **Data Science with Python** course and utilizes **scikit-learn**, **Matplotlib**, **Seaborn**, and **Pandas** for data analysis and visualization.

## Features
### 1. Weather Prediction
- Users can input **Month, Year, and Temperature** to predict **Rainfall**.
- Alternatively, users can input **Month, Year, and Rainfall** to predict **Temperature**.
- The model is trained once using historical weather data from **1901 to 2023**.
- Uses **Linear Regression** from **scikit-learn**.

### 2. Weather Visualization
- Users can upload a dataset (CSV, XLSX) containing columns: **Year, Month, Rain, Temperature**.
- The application generates various graphs like:
  - Rainfall vs. Temperature
  - Monthly Rainfall Trends
  - Yearly Temperature Changes
  - Other statistical insights.

### 3. Weather Analysis
- Uses **Linear Regression and K-Means Clustering** to analyze patterns such as:
  - **Which months have the highest/lowest rainfall?**
  - **Which years had extreme weather conditions?**
  - **Temperature trends over the years.**
  - **Seasonal variations in rainfall and temperature.**

## Technologies Used
### Programming Languages & Frameworks
- **Python** (Backend logic, Machine Learning, Data Processing)
- **Django** (Web Framework)
- **JavaScript, HTML, CSS** (Frontend)
- **Jupyter Notebook** (Model training & Data analysis)

### Libraries & Tools
- **Pandas** (Data handling)
- **Matplotlib & Seaborn** (Visualization)
- **scikit-learn** (Machine Learning models: Linear Regression, K-Means Clustering)
- **Joblib** (Model persistence for predictions)

## Installation & Setup
### Prerequisites
Ensure you have **Python 3.7+** and **pip** installed. Then, install the required dependencies:
```sh
pip install django pandas matplotlib seaborn scikit-learn joblib
```

### Run the Project
1. Clone this repository:
```sh
git clone https://github.com/yourusername/weather-prediction-app.git
cd weather-prediction-app
```
2. Run Django migrations:
```sh
python manage.py migrate
```
3. Start the development server:
```sh
python manage.py runserver
```
4. Open your browser and go to:
```
http://127.0.0.1:8000/
```

## Project Structure
```
weather-prediction-app/
│── myapp/
│   │── templates/
│   │── static/
│   │── views.py
│   │── models.py
│   │── urls.py
│── static/
│   │── dataset/weather_dataset.csv
│── trained_models/
│   │── temp_model.joblib
│   │── rain_model.joblib
│── db.sqlite3
│── manage.py
│── requirements.txt
│── README.md
```

## How to Use the App
### 1. Weather Prediction
- Navigate to **Weather Prediction** page.
- Choose between **Rainfall Prediction** or **Temperature Prediction**.
- Enter the required input values.
- Click **Predict** to get results.

### 2. Weather Visualization
- Go to **Weather Visualization**.
- Upload a dataset (CSV or XLSX).
- Click **Upload** to generate graphs.

### 3. Weather Analysis
- Navigate to **Weather Analysis**.
- Upload a dataset.
- Get insights using **Regression and Clustering models**.

## Dataset
The dataset used for training and analysis was collected from **Kaggle**, containing historical weather data from **1901 to 2023**.

## License
This project is open-source and available under the **MIT License**.

## Author
**Md. Rasel Molla**
