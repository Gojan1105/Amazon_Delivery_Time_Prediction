# Amazon Delivery Time Prediction

## Naan Mudhalvan
### 1105 - Gojan School of Business and Technology  
**Course Name**: Data Analytics in Process Industry  
**Project Title**: Amazon Delivery Time Prediction

### Submitted by:
- **Indhumathi.G** - 110523237006  
- **Indusha.S** - 110523237007  
- **Jayashree.J** - 110523237008  
- **Kaviya.V** - 110523237011  
- **Kavya.T** - 110523237012  

## Project Overview
This project aims to predict delivery times for e-commerce orders based on various factors such as product size, distance, traffic conditions, weather, and shipping method. By analyzing a dataset of Amazon delivery orders, we develop regression models to estimate the time it takes for an order to be delivered. The final application provides a user-friendly interface for users to input relevant details and get predicted delivery times.

## Skills Learned
- Python Scripting
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Machine Learning (Regression Modeling)
- MLflow (Model Tracking)
- Streamlit (Frontend Development)

## Domain
- **E-Commerce**
- **Logistics**

## Problem Statement
The objective is to predict the delivery time of e-commerce orders using features such as:
- Product size
- Distance between store and delivery address
- Traffic conditions
- Weather during delivery
- Shipping method
- Agent rating

The goal is to build a regression model that can predict delivery times accurately and create an interactive web application for users to input order details and receive delivery time predictions.

## Business Use Cases
1. **Enhanced Delivery Logistics**: Improve customer satisfaction and optimize delivery schedules.
2. **Dynamic Traffic and Weather Adjustments**: Update delivery time predictions based on real-time traffic and weather conditions.
3. **Agent Performance Evaluation**: Assess delivery agent performance and improve efficiency.
4. **Operational Efficiency**: Optimize resource allocation by analyzing delivery trends and performance metrics.

## Approach

### 1. **Data Preparation**
   - Load and preprocess the dataset.
   - Handle missing or inconsistent data.
   - Perform feature engineering (e.g., calculate distances between store and drop locations).

### 2. **Data Cleaning**
   - Remove duplicates and handle missing values.
   - Standardize categorical variables (e.g., weather, traffic).

### 3. **Exploratory Data Analysis (EDA)**
   - Analyze delivery times, agent performance, and external factors (traffic, weather).
   - Visualize trends and relationships in the dataset.

### 4. **Feature Engineering**
   - Calculate geospatial distances between store and drop-off coordinates.
   - Extract time-based features (e.g., hour of day, day of the week).

### 5. **Model Development**
   - Train multiple regression models, including:
     - Linear Regression
     - Random Forest Regressor
     - Gradient Boosting Regressor
   - Evaluate models using metrics like RMSE, MAE, and R-squared.
   - Track models and performance metrics using **MLflow**.

### 6. **Streamlit Application Development**
   - Build an interactive user interface for users to input order details (e.g., distance, traffic, weather).
   - Display predicted delivery times based on the model's predictions.

### 7. **Model Comparison and Tracking**
   - Use **MLflow** to log, compare, and track different models.
   - Document hyperparameters, performance metrics, and model versions.

### 8. **Deployment**
   - Deploy the model and application on **Streamlit** for public access and scalability.

## Dataset
**amazon_delivery.csv**: The dataset contains detailed information about orders, agents, and delivery conditions.

### Dataset Features:
- **Order_ID**: Unique identifier for each order.
- **Agent_Age**: Age of the delivery agent.
- **Agent_Rating**: Rating of the delivery agent.
- **Store_Latitude/Longitude**: Geographic location of the store.
- **Drop_Latitude/Longitude**: Geographic location of the delivery address.
- **Order_Date/Order_Time**: Date and time when the order was placed.
- **Pickup_Time**: Time when the order was picked up by the agent.
- **Weather**: Weather conditions during delivery.
- **Traffic**: Traffic conditions during delivery.
- **Vehicle**: Mode of transportation used for delivery.
- **Area**: Type of delivery area (Urban/Metropolitan).
- **Delivery_Time**: Target variable representing the actual time taken for delivery (in hours).
- **Category**: Product category of the order.

## Key Visualizations
- **Bar charts**: Distribution of delivery times by product category.
- **Scatter plots**: Relationship between distance and delivery time.
- **Heatmaps**: Correlations between weather, traffic, and delivery time.

## Results
By the end of this project, the following will be achieved:
- A cleaned and processed dataset ready for modeling.
- Multiple regression models developed and tracked using **MLflow**.
- Insights into the factors influencing delivery times.
- A fully functional delivery time prediction system, accessible via a **Streamlit** application.

## Installation

### Prerequisites:
Make sure you have Python 3.7+ installed. You will also need to install the following Python libraries:

```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn streamlit mlflow
