# NBA-Over-Under-Predictor
Predicting whether an NBA game will go Over or Under its total points line. Our goal is over 52.5% accuracy, above which a bettor will turn a profit.

## Sources

Game Data:
- https://www.basketball-reference.com/

Historical Odds:
- https://www.sportsbookreviewsonline.com/scoresoddsarchives/nba/nbaoddsarchives.htm

## Process

1. Gather data.
2. Clean and prepare data for model pre-processing & feature engineering.
3. Split dataset into train/validation & test sets.
4. Model training data and validate.
5. Compare model performances in order to select a model to tune for final implementation.

## Results

- 5 different models were explored with varying levels of success (cross-validated accuracy reported):
  - Logistic Regression: 50.1%
  - Decision Tree: 50.4%
  - Random Forest: 50.1%
  - XGBoost: 49.5%
  - Bagged Decision Tree: 49.4%
  
## Future Work

- Engineer new features that are more correlated to our target.
- Use PCA to see if any insights can be drawn from our "snapshot" features (rolling average statistics).
- Perhaps change from a classification approach to a regression one, comparing the line and predicted points scored.
- Find odds & lines that go pre-2007 season.
- Deploy web application that gives a recommendation (classification result) based on a selected game from the schedule.
