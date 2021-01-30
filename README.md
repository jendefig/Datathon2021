# Datathon2021
Datathon 2021 Repository 

```
- notebooks
- raw_data             <-- do NOT check in; keep in your local folders only
   |- DataDictionary*.csv
   |- Training*.csv

# Jeny's Submissions
Submission 1
   In this submission I dropped all columns with over 40% missing values and ran through Catboost. 
   Score on Kaggle: 0.84172

Submission 2
   In this submission, I deleted 72 features determined not useful after looking at charts from my SweetViz notebook and/or because of excessive missing data.
   I then did feature engineering to include but reduce the categories for hospital_id and icu_id, counting their frequencies of encounters and binning hospitals
   and icus into 1-3 and 1-5, respectively smallest to largest.  These new features are named hospital_size and icu_size
   Next I used KNNImputer to impute the missing data.
   Finally the model was again trained with Catboost.
   Score: 0.49744

Submission 3/4
   fail in code and setting up
   Score:  0.50456

Submission 5
   Removed lower 89ish of feature importances from Sub 2
   Score: 0.49744

Submission 6
   Trying out featurewiz and autoviml
   Score: 0.85176

