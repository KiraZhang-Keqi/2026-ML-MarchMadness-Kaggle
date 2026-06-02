# NCAA Tournament Outcome Prediction System

## Overview

Developed an end-to-end machine learning pipeline to predict NCAA tournament game outcomes using over 20 years of historical basketball data.

The project combines feature engineering, team rating systems, predictive modeling, probability calibration, and large-scale inference to generate win probabilities for every possible tournament matchup.

### Key Achievements

* Processed 210,000+ historical NCAA games
* Engineered 53 predictive features from multiple data sources
* Built a two-stage machine learning framework using XGBoost and Logistic Regression
* Implemented Leave-One-Season-Out validation to prevent temporal leakage
* Generated 132,133 tournament matchup predictions
* Achieved a Brier Score of 0.1679


## Business Objective

Accurately estimating game outcomes is valuable for tournament forecasting, sports analytics, and probabilistic decision-making.

This project focuses on predicting matchup win probabilities by combining historical performance, team quality metrics, schedule strength, and recent momentum into a unified predictive framework.


### Sources

* NCAA Regular Season Results (2003–2025)
* NCAA Tournament Results
* Team Seeding Information

### Scale

| Metric               | Value   |
| -------------------- | ------- |
| Historical Seasons   | 22      |
| Regular Season Games | 208,280 |
| Tournament Games     | 2,410   |
| Matchups Predicted   | 132,133 |
| Features Engineered  | 53      |

## Methodology

### Feature Engineering

Created 53 features across seven feature groups:

#### Performance Metrics

* Offensive Rating
* Defensive Rating
* Effective Field Goal Percentage
* Turnover Rate
* Rebounding Rate
* Free Throw Rate

#### Context Features

* Head-to-Head Performance
* Recent Team Momentum
* Away Game Success Rate
* Tournament Seed Information

### Modeling Pipeline

```text
Raw NCAA Data
      ↓
Data Cleaning
      ↓
Feature Engineering
      ↓
XGBoost Margin Prediction
      ↓
Probability Calibration
      ↓
Ensemble Modeling
      ↓
Tournament Win Probabilities
```

### Validation Strategy

Implemented Leave-One-Season-Out Cross Validation, where each season is held out as an independent test set. This approach better simulates real-world forecasting and prevents information leakage from future seasons.


## Results

| Metric            | Result               |
| ----------------- | -------------------- |
| Brier Score       | 0.1679               |
| Seasons Evaluated | 22                   |
| Prediction Range  | 0.034 – 0.974        |
| Validation Method | Leave-One-Season-Out |

The model demonstrated stable performance across multiple seasons, indicating robustness to changing tournament dynamics and team compositions.


## Technologies

### Machine Learning

* XGBoost
* Scikit-Learn
* StatsModels

### Development

* Jupyter Notebook
* Git
* GitHub

## Skills Demonstrated

* Data Cleaning and Transformation
* Feature Engineering
* Predictive Modeling
* Machine Learning Evaluation
* Cross Validation Design
* Statistical Modeling
* Probability Calibration
* Data Pipeline Development
* Exploratory Data Analysis
* Model Interpretation

## Repository Structure

```text
├── 2026NCAA Final Submission.ipynb
├── 2026NCAA Experiments.ipynb
├── 2026NCAA Predictions.csv
└── README.md
```

```
```
