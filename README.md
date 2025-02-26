
# **New York Taxicab Fare Prediction**  

## **Project Overview**  
This project focuses on predicting taxi fares in New York City using machine learning techniques. The dataset, collected from the **TLC New York City Taxi Data Collection (2016)**, contains trip details such as pickup and drop-off locations, timestamps, distance traveled, and fare amounts.  

## **Dataset Information**  
- **Source:** [Kaggle - NYC Yellow Taxi Trip Records (2023)](https://www.kaggle.com/datasets/nagasai524/nyc-taxi-trip-records-from-jan-2023-to-jun-2023)  
- **Timeframe:** February 2016  
- **Shape:** `(500,000 rows × 12 columns)`  
- **Attributes:**  
  - **Trip details** (pickup/drop-off time, location, distance)  
  - **Fare amount and extra charges**  
  - **Payment method**  
  - **Passenger count**  

## **Objective**  
The goal is to build a **machine learning model** that accurately predicts taxi fares based on trip details.  

## **Approach & Methodology**  
1. **Data Preprocessing**  
   - Handle missing values and outliers  
   - Feature engineering (e.g., extracting day, hour, distance calculation)  

2. **Exploratory Data Analysis (EDA)**  
   - Identify correlations between fare amount and other features  
   - Visualize data distribution  

3. **Model Selection & Training**  
   - **Baseline Model:** Linear Regression  
   - **Advanced Models:** Decision Trees, XGBoost  
   - **Performance Metrics:** RMSE, R², MAPE  

## **Results**  
| Model | RMSE | R² | MAPE |  
|-----------------|------|------|------|  
| **Linear Regression** | 3.366 | 0.90 | 0.123 |  
| **Decision Tree** | 3.639 | 0.88 | 0.168 |  
| **XGBoost** | **2.760** | **0.93** | **0.175** |  

## **Dataset Attributes**  
| Feature | Description |  
|----------------|-----------------------------------------------------------------|  
| `VendorID` | TPEP provider (1= CMT, 2= VeriFone) |  
| `tpep_pickup_datetime` | Pickup time |  
| `tpep_dropoff_datetime` | Drop-off time |  
| `passenger_count` | Number of passengers |  
| `trip_distance` | Distance in miles |  
| `pickup_longitude` | Pickup longitude |  
| `pickup_latitude` | Pickup latitude |  
| `RateCodeID` | Rate type (e.g., Standard, JFK, Newark) |  
| `store_and_fwd_flag` | If data was stored before transmission |  
| `payment_type` | Payment method (1=Credit card, 2=Cash, etc.) |  
| `fare_amount` | Base fare amount |  
| `extra` | Additional charges |  
| `mta_tax` | NYC MTA tax |  
| `improvement_surcharge` | Mandatory fee |  
| `tip_amount` | Tip (if applicable) |  
| `tolls_amount` | Toll fees |  
| `total_amount` | Final fare charged |  

## **Technologies Used**  
- **Python** (Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn)  
- **Jupyter Notebooks** for analysis and visualization  
- **Machine Learning Models** for predictive analytics  

## **How to Run the Project**  
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/nyc-taxi-fare-prediction.git
   cd nyc-taxi-fare-prediction
