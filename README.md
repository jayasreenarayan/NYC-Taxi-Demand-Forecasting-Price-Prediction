🚕 NYC Taxi Fare Prediction
--
Project Title: NYC Taxi Demand Forecasting & Price Prediction
Objective: Build a robust model to predict NYC taxi fares based on trip data to improve transparency, optimize pricing, and support planning.

📌 Overview:
--
Accurate fare prediction is crucial for passengers, drivers, and ride-hailing platforms in New York City. Taxi fare depends on multiple factors like trip distance, time of day, pickup/dropoff location, and surcharges.

This project leverages historical Yellow Taxi trip data from the NYC Taxi and Limousine Commission (TLC) to analyze ride patterns and build a predictive model using regression techniques. The goal is to deliver a reliable fare estimation tool that enhances rider trust, assists drivers in route planning, and supports data-driven decision-making for taxi operators and urban planners.

📂 Data Source:
--
We use publicly available NYC Yellow Taxi trip data provided by the NYC Taxi & Limousine Commission (TLC).

Key Features:
trip_distance: Distance traveled (miles)

pickup_datetime & dropoff_datetime: Enables extraction of:

Trip duration

Day of the week

Time of day

PULocationID, DOLocationID: Geographic zones

fare_amount: Target variable

extra, mta_tax, tip_amount, tolls_amount, total_amount: Additive fare components

🔍 Exploratory Data Analysis (EDA):
--
We begin with descriptive analysis to understand how fares relate to trip features:

Distance vs Fare Scatterplots

Temporal Trends (peak hour, weekday/weekend analysis)

Fare distributions by pickup/dropoff zones

Outlier handling and data cleaning

🧠 Modeling Approach
💡 Regression Model

Multiple Linear Regression:

Predictors: Trip distance, trip duration, time of day, pickup/dropoff zones

Encoded categorical variables for location IDs and temporal bins

Advanced Models (optional):

Random Forest

XGBoost

Gradient Boosting

🧪 Evaluation Metrics:
--
RMSE (Root Mean Square Error)

MAE (Mean Absolute Error)

R² Score

📈 Project Outcomes
--
🚖 Accurate Fare Predictions: Estimate fare before a ride starts using trip characteristics.

💰 Pricing Transparency: Improve user trust through fair pricing and better communication.

📊 Operational Insights: Identify patterns by location and time to support driver incentives or pricing strategies.

🏙️ Urban Planning: Understand travel behaviors to support city planning and infrastructure development.

🛠️ Tech Stack
--
Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost

Environment: Jupyter Notebooks / Google Colab

Visualization Tools: Plotly, seaborn, matplotlib

📅 Next Steps
--
Include weather and traffic data for improved predictions

Expand to include Green/For-Hire taxis and ride-share apps

Deploy model via API for real-time fare predictions


pip install -r requirements.txt
