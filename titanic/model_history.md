# Model 2:
Model Type:
- Xgboost

Notes:
This version wont be anything fancy. We'll simply
- DROP Colunms highly correlated columns with lots of NULL values and d
    - SibSp
    - Cabin
- Drop NULL  Rows from columns that have few nulls:
  - fare
  - embarked
- Drop Columns that need feature engineering
  - Ticker
