# Rainfall Prediction Model

An end-to-end machine learning web application that predicts the likelihood of rainfall based on real-time meteorological data. 
This project bridges a robust Python backend with a responsive frontend, utilizing a Random Forest Classifier to achieve an 86% prediction accuracy.

## Tech Stack

**Frontend**
* HTML5, CSS3, JavaScript
* Tailwind CSS (for responsive styling)
* OpenWeatherMap API (Real-time data fetching)

**Backend & Machine Learning**
* Python 3.x
* Flask (RESTful API development)
* Scikit-Learn (Model training & evaluation)
* Pandas & NumPy (Data preprocessing and feature engineering)
* Joblib / Pickle (Model serialization)

## Key Features

* Real-time weather data fetching
* User geolocation support
* Machine learning classification model
* Instant prediction results and probabilities
* Responsive UI layout

## 🏗️ System Architecture

1. Data Collection & Preprocessing: Historical weather data was cleaned, normalized, and processed using Pandas. Missing values were handled, and features like dew point were calculated.
2. Model Training: A Random Forest Classifier was trained on parameters including atmospheric pressure, temperature, dew point, humidity, and wind speed. 
3. API Layer: A Flask backend serves the serialized `.pkl` model. It exposes a `/api/predict` endpoint that accepts JSON payloads of weather parameters and returns prediction confidence scores.
4. Client Interface: The browser-based UI collects data (either manually entered or via API) and asynchronously communicates with the Flask backend to render results instantly.

## Local Setup

1. Clone the repository
2. Install the required dependencies: `pip install -r requirements.txt`
3. Add your OpenWeatherMap API key in the code
4. Run the application: `python app.py`
5. Open `http://127.0.0.1:5000` in your browser

👨‍💻 Author
Saurav Kadam
LinkedIn
Full Stack Developer | B.Tech Artificial Intelligence & Data Science
