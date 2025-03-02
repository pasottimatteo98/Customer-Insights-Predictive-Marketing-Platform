# Customer Insights & Predictive Marketing Platform

## Overview
This repository contains two Python scripts for comprehensive marketing analytics. The scripts analyze customer behavior, predict churn, perform sentiment analysis on reviews, conduct RFM (Recency, Frequency, Monetary) analysis, and identify purchase patterns through market basket analysis.

## Files
- `marketing.py`: Core analysis script with churn prediction and RFM analysis
- `progetto_marketing.py`: Extended analysis including sentiment analysis and market basket analysis

## Features

### Customer Segmentation and RFM Analysis
- Segments customers based on purchase recency, frequency, and monetary value
- Creates customer segments: Top Customers, High Value Customers, Medium Value Customers, Low Value Customers, and Lost Customers
- Visualizes customer segments with pie charts

### Churn Prediction
- Defines churn based on purchase timing patterns
- Implements multiple machine learning models:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
  - Decision Trees
- Compares model performance with metrics like accuracy, precision, recall, and F1-score

### Sentiment Analysis
- Uses both custom LSTM model and pre-trained BERT for review classification
- Processes text data with stemming, lemmatization, and stop word removal
- Classifies reviews as positive, negative, or neutral
- Visualizes sentiment distribution across customer segments

### Market Basket Analysis (MBA)
- Identifies product associations using the Apriori algorithm
- Analyzes:
  - Product class associations
  - Product ID associations
  - Associations by loyalty type
  - Associations by customer segment
- Visualizes association rules with network graphs and heatmaps

## Requirements
The scripts use Python libraries including:
- pandas
- numpy
- scikit-learn
- TensorFlow
- NLTK
- mlxtend
- matplotlib
- seaborn
- networkx

## Dataset
The scripts work with a marketing analytics dataset containing:
- Customer accounts
- Customer information
- Product details
- Order history
- Customer reviews

## Usage
To use these scripts:
1. Ensure you have all required libraries installed
2. Prepare the dataset files in the same directory as the scripts
3. Run the scripts in a Python environment with sufficient memory for model training

## Notes
- The scripts were originally developed in Colab notebooks
- Some scripts contain paths specific to Google Drive storage
- The BERT model requires significant computational resources
