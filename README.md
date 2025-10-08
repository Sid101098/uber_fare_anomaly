# uber_fare_anomaly
Uber Fare Anomaly Detection Project
This project generates a synthetic dataset of Uber trips and analyzes fare anomalies using machine learning.

Project Structure
generate_uber_dataset.py - Creates the synthetic Uber trip dataset

uber_fare_anomaly_analysis.ipynb - Jupyter notebook for data analysis and anomaly detection

uber_fare_anomalies.csv - Generated dataset file (created after running the script)

Dataset Description
The dataset contains 50,000 synthetic Uber trip records with the following columns:

trip_id: Unique identifier for each trip

datetime: Date and time of the trip

hour: Hour of the day (0-23)

day_of_week: Day of week (0=Monday to 6=Sunday)

distance_miles: Trip distance in miles

duration_minutes: Trip duration in minutes

pickup_lat, pickup_lng: Pickup location coordinates

dropoff_lat, dropoff_lng: Dropoff location coordinates

surge_multiplier: Surge pricing multiplier

fare_amount: Total fare amount in dollars

is_anomaly: Whether the fare is anomalous (1) or normal (0)

anomaly_type: Type of anomaly (overcharge, undercharge, distance_outlier, duration_outlier, or normal)

Prerequisites
Make sure you have Python installed along with these packages:

pandas

numpy

matplotlib

seaborn

scikit-learn

jupyter

Analysis Features
The notebook includes:

Data loading and basic information

Anomaly distribution analysis

Fare amount visualizations

Temporal analysis (by hour and day of week)

Correlation analysis

Anomaly detection using Isolation Forest algorithm

Model evaluation with confusion matrix

Feature importance analysis

PCA visualization of anomalies

Anomaly Types
The dataset includes four types of anomalies:

Overcharge: Fares that are 3x to 10x higher than normal

Undercharge: Fares that are 70-90% lower than normal

Distance Outlier: Trips with extremely long distances

Duration Outlier: Trips with extremely long durations

Expected Results
Dataset with approximately 5% anomalies (2500 anomalous records)

Isolation Forest model that can detect fare anomalies

Visualizations showing patterns in normal vs anomalous fares

Insights into which features are most important for anomaly detection

Use Cases
This project can be used for:

Learning about anomaly detection techniques

Understanding fare patterns in ride-sharing data

Practicing data analysis and machine learning with real-world scenarios

Developing fraud detection systems

Notes
The data is synthetic and generated for educational purposes

Actual Uber fare patterns may differ from this simulated data

The anomaly detection model can be improved with more sophisticated techniques

The project serves as a foundation for more advanced analysis
