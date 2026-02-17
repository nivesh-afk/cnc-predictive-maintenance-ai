# CNC Predictive Maintenance using Machine Learning

## 📖 Overview
This project presents an AI-driven predictive maintenance system for CNC machines.  
It integrates mechanical health scoring with machine learning models to estimate failure probability and assess system condition.

The objective is to reduce unexpected downtime, improve maintenance scheduling, and extend machine life using data-driven insights.



## 🎯 Project Objectives
- Develop a mechanical health scoring system (0–100 scale)
- Predict machine failure probability using Random Forest
- Visualize operational trends and degradation patterns
- Provide actionable maintenance insights
- Enable low-cost predictive maintenance for MSMEs



## 🏭 Machine Context
The project models a CNC spindle/tool system where critical parameters include:
- Air Temperature
- Process Temperature
- Rotational Speed (RPM)
- Torque
- Tool Wear
- Failure Status



## 📂 Dataset
Dataset used: AI4I 2020 Predictive Maintenance Dataset (Kaggle)

Features:
- Air_Temp
- Process_Temp
- RPM
- Torque
- Tool_Wear
- Target (Failure)
- Health_Score (engineered)
- Failure_Probability (predicted)



## ⚙️ Methodology

### 1️⃣ Health Score Calculation
A rule-based degradation model calculates health score based on:
- Temperature thresholds
- RPM anomalies
- Tool wear levels
- Torque stress

Score range: 0 (critical) – 100 (healthy)



### 2️⃣ Machine Learning Model
Model Used: Random Forest Classifier

Reasons:
- Handles small to medium datasets effectively
- Robust to noise
- Provides feature importance
- Good performance for binary failure prediction

Outputs:
- Failure prediction (0/1)
- Failure probability (0–1)



## 📊 Visualizations

The system generates:
- Health Score Distribution
- Failure Distribution
- RPM vs Torque Relationship
- Tool Wear vs Failure Probability
- Correlation Matrix
- Feature Importance Graph

These visualizations help interpret machine degradation patterns.



## 📈 Key Results
- Average Health Score ≈ 80 (Moderate condition)
- Clear correlation between tool wear and failure probability
- Failure probability increases significantly when health score < 40
- Model achieves strong classification accuracy on test data



## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SQLite (for database integration)



## 💡 Practical Impact

- Potential downtime reduction: 30–50%
- Early detection of mechanical degradation
- Cost savings for MSMEs (₹50,000–₹1,00,000 per machine annually)
- Prevents bearing seizure and spindle failure



## 🔮 Future Scope

- Integration with IoT vibration sensors
- CNN-based oil image analysis
- Remaining Useful Life (RUL) prediction using LSTM
- Real-time dashboard implementation



