<h1 align="center">✈️ Flight Price Prediction</h1>


A **machine learning pipeline** for predicting **domestic flight ticket prices** in India by transforming raw **itinerary data** into structured, model-ready features.  
The project focuses on **robust feature engineering**, **data cleaning**, and **encoding** to prepare a high-quality dataset for regression models.

## What the Pipeline Does
- **Loads & merges** training and test datasets for consistent preprocessing  
- **Extracts** useful features from messy text fields: **dates**, **times**, **routes**, **stops**, and **durations**  
- **Normalizes & encodes** categorical data like **airline**, **source**, and **destination**  
- **Handles missing values** and **removes anomalies** (e.g., unrealistically short durations)  
- **Outputs** a tidy dataset ready for model training and prediction

## Key Feature Engineering
- **Calendar features:** Extract **day**, **month**, **year** from journey dates  
- **Time-of-day features:** Separate departure and arrival into **hour** and **minute** components  
- **Stops normalization:** Convert text labels (e.g., *non-stop*, *1 stop*) into numeric counts  
- **Duration parsing:** Convert "Xh Ym" strings into numeric **hour** and **minute** columns, handling edge cases  
- **Categorical encoding:** Apply label encoding to airline, source, destination, and additional info

## Why It Matters
Flight prices depend on **seasonality**, **time of day**, **number of stops**, **duration**, and **airline preferences**.  
This pipeline captures those relationships in a form that machine learning models can use to **predict pricing patterns** accurately.



