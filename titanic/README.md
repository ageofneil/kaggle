# Titanic Survivor Classification

This readme contains my observations, notes, and ideas on how to solve
this classification problem.

## The Data

Key points to remeber:

- 8.1% of data is missing. Will need to figure out how to deal with this.
- total of 12 variables
  - PassengerId: DROP
  - Survived: Target
  - Pclass:
    - type: Catgorical (3,1,2)
    - null: 0
  - Name:
    - type: Categorical
    - Null: 0
    - Notes: Name's wont mean much unless we can do some feature engineering. Drop
from first versions of model and come back to this later if we have time to feature
engineer.
  -  Sex:
    - Type: Categorial
    - Null: 0
  - Age:
    - Type: Numirical (ordinal)
    - Missing: 20%
    - Notes: What to do with missing???
       - Don't use feature (probaly not good as age should be important)
       - remove the columns (to much.. 20%..)
       - **Leave it null... this will work for tree models**
       - Fill it with a mean or more (similar to leave it null)
       - Imputation: Make a model to predict age. (worth trying if time permets.)
  - SibSpa: # of siblings / spouses aboard the Titanic
    - Numerical: Ordinal
    - Null: 68%
    - Notes: What to do with NUlls? We can assume that nulls means 0 (no family).
    if time permits we can possibly use name to try and fill out some nulls, and an
    imputation model.
  - Parch: # of parents / children aboard the Titanic
    -  Numerical (ordinal)
    -  Missing:  76%
    -  Notes: Could probably feature engineer with name + sibspa
  - Ticket:
    - 681 Values. Will need feature engineering.
    - Nulls:  0
  - Fare:
    - Type: Numeric
    - Missing: 2%
      - Only 2%... Let's drop missing columns
  - Cabin:
    - Type:  Categorical
    - Distinc: 72%
    - Missing: 77%
    - Notes: Correlated with Fate. Probably need to do some NLP to feature engineer.
  - Embarked: Categorical, DROP missing.


## Model 1 (BASIC) todos:'
- NULLS:
 - Embarked
'


