# Bus Arrival Time Prediction using Machine Learning

## Project details
- **Student allocation:** Question 29
- **Project title:** Bus Arrival Time Prediction
- **Dataset named in the allocation sheet:** Bus Travel Time Dataset
- **Algorithm category:** Regression
- **Target/output:** Travel/arrival time
- **Objective:** Predict estimated bus travel time from route, distance, departure hour, day, weather, traffic and number of stops.

## Important dataset note
The uploaded allocation PDF identifies the dataset by name but does not contain the actual dataset file. To make this GitHub project runnable, `bus_travel_time_dataset.csv` is an **illustrative synthetic dataset generated for demonstration**. If your instructor supplied an official Bus Travel Time Dataset separately, use that file instead and adjust the column names in the code as needed.

## Files
- `bus_arrival_time_prediction.py` — complete training and evaluation code
- `bus_travel_time_dataset.csv` — illustrative dataset (600 records)
- `Bus_Arrival_Time_Prediction_Report.pdf` — project report

## Features
- Route
- Distance_km
- Departure_Hour
- Day_of_Week (0 = Monday, 6 = Sunday)
- Weather
- Traffic_Level
- Number_of_Stops

## Target
- `Travel_Time_min` — estimated trip travel time in minutes

## Requirements
Python 3.9+
```bash
pip install pandas numpy scikit-learn
```

## Run
Keep the CSV and Python file in the same folder, then run:
```bash
python bus_arrival_time_prediction.py
```

## Workflow
1. Load and inspect data
2. Remove duplicate rows and missing values
3. Encode categorical features using One-Hot Encoding
4. Split into training and testing data (80:20)
5. Train a Random Forest Regressor
6. Evaluate using MAE, RMSE and R-squared
7. Predict travel time for a new bus trip
