# IPL Victory Probability Estimator

## 🎯 Project Overview

This project is an end-to-end data science application designed to predict the victory probability of teams in Indian Premier League (IPL) cricket matches. It utilizes a machine learning pipeline, meticulously crafted from an extensive historical IPL dataset, to provide real-time, data-driven forecasts for cricket enthusiasts and analysts. The goal is to offer a deeper, more engaging way to follow the game by predicting which team is likely to win at any given point during a match.

---

## 🛠 Methodology

The project's workflow is structured into several key phases:

* *Data Sourcing & Cleaning:* The project begins with a comprehensive analysis of a historical IPL dataset, which includes ball-by-ball and match-level data. This raw data is cleaned, preprocessed, and transformed using the Python pandas library within a Jupyter Notebook environment.
* *Feature Engineering:* Relevant features are engineered from the raw data to capture key factors influencing a match's outcome, such as team performance, venue conditions, recent form, and live in-game statistics like runs scored and wickets fallen.
* *Model Training:* A machine learning model is trained on this prepared dataset to identify complex patterns and relationships that lead to victory. The model learns to predict the win probability of the batting team at each stage of a match.
* *Model Serialization:* The entire machine learning pipeline, including the trained model and all necessary data transformation steps, is serialized using the pickle library. This allows for the efficient storage and retrieval of the model, eliminating the need to retrain it every time the application is run.

---

## 🚀 Live Application

To make the predictive model accessible and easy to use, it is deployed as an interactive web application built with *Streamlit*. The application provides a simple and intuitive interface where users can input real-time match details—such as the teams playing, the city, and the current score—to receive an instant forecast of each team’s victory probability. The web app dynamically displays these probabilities, complete with a progress bar, offering a clear and engaging visualization of the prediction.

---

## 📂 Project Files

* app.py: The main Python script for the Streamlit web application.
* deliveries.csv & matches.csv: The raw historical IPL datasets used for analysis and model training.
* IPL_Win_Prob.ipynb: The Jupyter Notebook containing the full code for data cleaning, feature engineering, and model training.
* model.pkl & pipe.pkl: The serialized machine learning model and pipeline, saved using pickle.
* city.pkl & team.pkl: Serialized data containing lists of unique cities and teams, used by the application for data preprocessing.

---

## 🤝 Contribution

Feel free to explore the code, open issues, or suggest improvements. This project is a demonstration of a complete data science workflow, from raw data to a live, predictive service.
