<<<<<<< HEAD
🏢 Building Energy Anomaly Detection using Machine Learning

📌 Project Overview

Energy consumption monitoring is critical for modern buildings to ensure operational efficiency, reduce costs, and detect abnormal behavior. Unexpected spikes or drops in electricity usage may indicate equipment malfunction, inefficiencies, or potential system failures.
This project focuses on detecting anomalies in hourly electricity consumption data using Machine Learning techniques. By applying multiple anomaly detection models and combining them through an ensemble approach, the system identifies abnormal energy patterns and estimates their financial impact.

🎯 Problem Statement

Buildings generate large volumes of time-series energy consumption data. Manual monitoring of such data is impractical. The goal of this project is to:
Detect unusual electricity usage patterns automatically.
Identify spike and drop anomalies.
Analyze seasonal and hourly anomaly trends.
Estimate the financial impact of anomalous energy usage.
This solution provides actionable business insights to reduce operational costs and improve energy efficiency.

📊 Dataset Description

The dataset contains:
Hourly electricity consumption readings.
Multiple building-level energy measurements.
Timestamp-based time-series data.
For analysis, a high-usage building was selected to ensure meaningful anomaly detection results.
Key Data Characteristics:
Hourly frequency
Multi-building energy readings
Time-series format
Two-year observation period

🛠️ Methodology
The project follows a structured machine learning workflow:

1️⃣ Data Preprocessing
Converted timestamp column to datetime format.
Set timestamp as index.
Selected individual building for analysis.
Handled missing values.

2️⃣ Feature Engineering
Created time-series features including:
Hour of day
Month
Day of week
24-hour rolling mean
24-hour rolling standard deviation
Lag features (1-hour and 24-hour)
These features help capture seasonality, trends, and short-term variations.

3️⃣ Anomaly Detection Models
Three different methods were applied:
🔹 Isolation Forest
Tree-based model that isolates anomalies based on random partitioning.
🔹 Local Outlier Factor (LOF)
Density-based method detecting points with lower local density.
🔹 Robust Z-Score
Statistical method using Median Absolute Deviation (MAD) to detect extreme deviations.

4️⃣ Ensemble Method
An observation is classified as an anomaly if at least two models agree.
This improves detection reliability and reduces false positives.

📈 Model Evaluation & Visualization

The following analyses were performed:
Feature importance using Random Forest.
Anomaly distribution by hour.
Seasonal anomaly analysis (monthly pattern).
Electricity usage visualization with anomaly highlights.
Classification of anomaly types (Spike vs Drop).
All visualizations are saved in the outputs/ folder.

💰 Business Insights & Financial Impact

To estimate financial impact:
Electricity price assumed: ₹6 per kWh.
Excess anomalous energy usage calculated.
Financial loss estimated using anomaly energy consumption.

Key Insights:

Peak anomaly hours identified.
Seasonal anomaly trends observed.
Spike anomalies contributed more to cost impact.
Potential cost savings identified by eliminating abnormal spikes.
This analysis demonstrates how anomaly detection can directly support business decision-making.

📂 Project Structure

Building_Energy_Anomaly_Detection/
│
├── data/
│   └── electricity.csv
│
├── notebooks/
│   └── energy_analysis.ipynb
│
├── outputs/
│   ├── energy_anomalies.png
│   ├── anomaly_distribution.png
│   ├── feature_importance.png
│
├── README.md
├── requirements.txt

▶️ How to Run the Project

Clone the repository:
git clone <repository-link>
Navigate to the project directory:

cd Building_Energy_Anomaly_Detection
Install required dependencies:

pip install -r requirements.txt
Open Jupyter Notebook:

jupyter notebook
Run energy_analysis.ipynb

🚀 Technologies Used

Python
Pandas
NumPy
Scikit-learn
Matplotlib
Jupyter Notebook

📌 Key Learnings

Practical implementation of unsupervised anomaly detection.
Feature engineering for time-series data.
Ensemble modeling improves reliability.
Business interpretation of machine learning results.
Translating technical findings into financial impact.

🔮 Future Improvements

Incorporate weather data for contextual anomaly detection.
Use deep learning models (LSTM Autoencoders).
Deploy as a real-time monitoring dashboard.
Implement alert system for live anomaly detection.

👩‍💻 Author

RAJUGANI PADMAVATHI

Building Energy Anomaly Detection
Machine Learning | Time-Series Analysis | Business Analytics
=======
# Building-Energy-Anomaly-Detection

## Overview
This project detects abnormal energy consumption patterns using machine learning techniques.

## Dataset
- Time-series electricity consumption dataset
- Hourly readings across multiple buildings

## Methodology
1. Data Cleaning
2. Feature Engineering
3. Rolling Statistics
4. Isolation Forest Model
5. Business Insight Analysis

## Model Configuration
- Isolation Forest
- Contamination: 2%
- Random State: 42

## Results
- ~1.98% anomalies detected
- Peak anomaly hours: 3 PM – 8 PM
- High anomaly months: July, August, January

## Business Insights
- Seasonal load impacts anomaly frequency
- Peak operational hours show higher instability

## Future Improvements
- Hyperparameter tuning
- Autoencoder-based anomaly detection
- Real-time dashboard deployment

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- 
>>>>>>> e49911d9053e2004636836d91cac1c0314b2f4c6
