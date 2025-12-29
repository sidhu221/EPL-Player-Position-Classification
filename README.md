# EPL Player Position Classification Using Machine Learning

## Overview
I used supervised machine learning to classify EPL player positions based on performance statistics. 

Using open-source data from 2023-2024 and 2024-2025 statistics, I trained and evaluated multiple models to predict a player's on-field role from statistical features

The project focuses on model generalization across seasons and real-world application to sports analytics. 

## Dataset
- Source: Public Kaggle Datasets
- Seasons Used:
  - 2023-2024: https://www.kaggle.com/datasets/orkunaktas/premier-league-all-players-stats-2324
  - 2024-2025: https://www.kaggle.com/datasets/aesika/english-premier-league-player-stats-2425
- Features Include:
  - Name, club, position, goals, assists, expected goals, expected assists, and more
 
## Tools & Technologies Utilized
- Python and Jupyter Notebook
- pandas and NumPy
- scikit-learn
- XGBoost
- Seaborn
- Matplotlib
 
## Problem Statement
#### Direct Scope: 
Using on-field statistics by different players with over 15 appearances, can we accurately classify a player's position (goalkeeper, defender, midfielder, forward)? 

#### Real-World Application: 
Many 3rd party statistical apps (FotMob, ESPN, Sleeper, EPL Fantasy) gather statistics from the Premier League directly, can I provide a solution to classify player position quickly using statistics with an accuracy of over 80%?

## Model Evaluation 
- Direct Accuracy (# of correct / total)
- Root Mean Squared Error (RMSE)

## Results
- Random Forest (2023-2024): **71% accuracy**
- Confusion Matrix (2023-2024): **80% accuracy**
- XGBoost (2023-2024): **81% accuracy**
- Random Forest (2024-2025): **85% accuracy**
- Confusion Matrix (2024-2025): **85% accuracy**
- XGBoost (2024-2025): **86% accuracy**

## Key Insights
- Clearances, tackles, goals, and appearances were the most impactful statistics in predicting position
- Defenders and Midfielders were the most misclassified position
### Reasoning
- Clearances and tackles distinguish a defender from a midfielder
- Goals distinguish a forward
- There are many hybrid midfielders that play a defensive midfield role, examples are Moises Caicedo and Declan Rice which have strong defensive statistics as a midfielder

## Limitations
- Positions in real-life are not discrete and coaches have their own role they create for a player
- There are many sub roles which are not included in the dataset (Wingers, Attacking Midfielders, and Defensive Midfielders)
- Dataset doesn't account for tactical and spatial contexts

## Future Work
- Add interactive visualizations or dashboards
- Apply the models to 2025-2026 EPL season


