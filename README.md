# DECODE-LABS: Data Science Internship

## Task 1: US Flight Delays, Advanced EDA & Feature Engineering
Notebook: [Task 1/Flight_Delays_Project.ipynb](Task%201/Flight_Delays_Project.ipynb)

- **Data:** 611,575 US domestic flights, June 2025 (US Bureau of Transportation Statistics)
- **Missing values:** filled based on their real-world reason, plus a Mean vs Median vs Group-median vs KNN experiment
- **Outliers:** IQR vs Z-score compared; extreme delays capped with Z-score (mean ± 3 std)
- **Features:** departure hour, time of day, weekend flag, aircraft's flight of the day, airport size, route

**Key finding:** a plane's 1st flight of the day is late 15% of the time; its 5th+ flight is late 42%+.

Data is not included (277 MB). Download June 2025 from https://www.transtats.bts.gov and save as `Task 1/data/flights_2025_06.csv`.

## Task 2: Credit Card Fraud Detection, Supervised Learning
Notebook: [Task 2/Fraud_Detection_Project.ipynb](Task%202/Fraud_Detection_Project.ipynb)

- **Data:** 284,807 card transactions, only 0.17% fraud (ULB Credit Card Fraud dataset)
- **Imbalance:** SMOTE inside an imblearn Pipeline, applied to training data only
- **Models:** Logistic Regression and Random Forest (scikit-learn), LR tuned with GridSearchCV
- **Evaluation:** Precision, Recall, ROC-AUC and PR-AUC (accuracy is misleading: 99.83% by always guessing "normal")

**Key result:** Random Forest + SMOTE caught 72 of 95 test frauds with only 6 false alarms out of 56,651 normal transactions (precision 0.92, ROC-AUC 0.968).

Data is not included (151 MB). Download `creditcard.csv` from https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud and save it in `Task 2/data/`.
