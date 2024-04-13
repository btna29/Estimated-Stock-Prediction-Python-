# Estimated-Stock-Prediction-Python-
Estimated Stock Prediction - Data Analytic Report
Introduction

This report details the exploratory data analysis (EDA) conducted for Gala Groceries, a technology-driven grocery store chain in the USA. Python and Google Colab were used to prepare data for training a machine learning model to predict stock levels. The findings and analysis were presented to the Cognizant engineering team and Gala Groceries' business representatives.

Purpose

The project aimed to optimize inventory levels for Gala Groceries, minimizing waste and stockouts.

Business Case

Gala Groceries prides itself on fresh, locally sourced produce, leading to challenges in maintaining consistent stock year-round. They require a data-driven approach to optimize inventory management for perishable groceries. Overstocking leads to waste and storage costs, while understocking risks losing customers.

Strategic Plan

Data Source: Data Engineering Team

Data Model:

The data model consists of three tables:

sales: Stores sales data.
sensor_storage_temperature: Captures IoT data from temperature sensors in storage facilities.
sensor_stock_levels: Provides estimated stock levels based on IoT sensors.
Relationships between tables are indicated by arrows, highlighting the linking columns for merging the datasets.

Analysis Insights:

Fruit and vegetables are the top two purchased categories.
Non-members are the most frequent customers.
Cash is the preferred payment method.
The busiest hour for transactions is 11am.
Action Plan

Data Preparation: Merge data based on the data model, followed by cleaning and outlier removal.
Feature Engineering: Create new features and transform datasets for predictive modeling.
Model Experimentation: Test various algorithms using cross-validation.
Evaluation and Iteration: Measure performance metrics and iterate on the model.
Production Algorithm Development: Develop the model as a production API.
Key Metric: estimated_stock_pct

A supervised machine learning model will be used, with estimated_stock_pct as the target variable to predict hourly stock levels.

Cross-Validation: A portion of the data will be withheld for testing the model's generalizability.

K-Fold Cross-Validation: The model will be trained and tested on multiple random samples (K folds) of the data to ensure robustness.

Trends Identified:

Unit price is a significant factor.
Product categories have less impact.
Unit price, temperature, and hour of day are crucial for predicting stock.
Conclusions:

Stock cheaper products more due to higher demand.
Increase stock levels with higher temperatures.
Adjust stock based on hour, quantity, and day of the month.
Recommendations:

Data Inclusion: Gather more data to address potential underfitting, where the model lacks sufficient examples for generalization.
Delivery Data: Include data on incoming deliveries to improve prediction accuracy.
Weather Data: Integrate weather data as buying patterns shift with weather changes.

