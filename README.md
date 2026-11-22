# DECODE-LABS: Data Science Internship

## Task 1: US Flight Delays, Advanced EDA & Feature Engineering
Notebook: [Task 1/Flight_Delays_Project.ipynb](Task%201/Flight_Delays_Project.ipynb)

- **Data:** 611,575 US domestic flights, June 2025 (US Bureau of Transportation Statistics)
- **Missing values:** filled based on their real-world reason, plus a Mean vs Median vs Group-median vs KNN experiment
- **Outliers:** IQR vs Z-score compared; extreme delays capped with Z-score (mean ± 3 std)
- **Features:** departure hour, time of day, weekend flag, aircraft's flight of the day, airport size, route

**Key finding:** a plane's 1st flight of the day is late 15% of the time; its 5th+ flight is late 42%+.

Data is not included (277 MB). Download June 2025 from https://www.transtats.bts.gov and save as `Task 1/data/flights_2025_06.csv`.
